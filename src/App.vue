<template>
  <v-app>

	<v-app-bar app color="primary">

	  <a href="/">
		<v-icon x-large dark>mdi-home</v-icon>
	  </a>

	  <v-spacer></v-spacer>

	  <nav class="navigation">
		<v-btn to="/groups/1" outlined dark>Младшая группа</v-btn>
		<v-btn to="/groups/2" outlined dark>Средняя группа</v-btn>
		<v-btn to="/groups/3" outlined dark>Старшая группа</v-btn>

		<v-btn to="/quizzes/create" outlined dark>Создать викторину</v-btn>
		<v-btn to="/quizzes/show" outlined dark>Проверка результатов</v-btn>
	  </nav>

	  <v-spacer></v-spacer>

	  <a href="/profile">
		<v-icon x-large dark>mdi-account-circle</v-icon>
	  </a>

	</v-app-bar>

	<v-main>
	  <router-view />
	</v-main>

  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend( {} )
</script>

<style>

.navigation {
  display: grid;
  grid-auto-flow: column;
  grid-gap: 20px;
}

</style>
