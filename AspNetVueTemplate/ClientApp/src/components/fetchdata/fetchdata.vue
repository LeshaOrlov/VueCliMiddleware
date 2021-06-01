<template>
    <div>
        <h1>Weather forecast</h1>

        <p>This component demonstrates fetching data from the server.</p>

        <v-simple-table v-if="forecasts.length">
            <template v-slot:default>
                <thead>
                    <tr>
                        <th>Date</th>
                        <th>Temp. (C)</th>
                        <th>Temp. (F)</th>
                        <th>Summary</th>
                    </tr>
                </thead>
                <tbody>
                    <tr v-for="item in forecasts" :key="item.id">
                        <td>{{ item.dateFormatted }}</td>
                        <td>{{ item.temperatureC }}</td>
                        <td>{{ item.temperatureF }}</td>
                        <td>{{ item.summary }}</td>
                    </tr>
                </tbody>
            </template>
        </v-simple-table>
    

    <p v-else><em>Loading...</em></p>
</div>
</template>

<script>
    export default {
        data() {
            return {
                forecasts: []
            }
        },

        mounted() {
            fetch('api/WeatherForecast')
                .then(response => response.json())
                .then(data => {
                    this.forecasts = data;
                });
        }
    }
</script>