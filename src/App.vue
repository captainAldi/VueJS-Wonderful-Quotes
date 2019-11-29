<template>
  <div id="app">
    <div class="container">
					<app-quoteGrid :quotes="quotes"></app-quoteGrid>
				</div>
  </div>
</template>

<script>
import QuoteGrid from './components/QuoteGrid.vue'

export default {
  name: 'app',
		data: function () {
			return {
				quotes: [
					'contoh quotes ke - 1'
				],
				quotesMaksimal: 10
			}
		},
		components: {
			'app-quoteGrid': QuoteGrid
		}
  
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
