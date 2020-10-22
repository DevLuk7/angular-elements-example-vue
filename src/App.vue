<template>
	<users-list :userslist="users" userSelect="userSelect"></users-list>;
</template>

<script>
	export default {
    name: 'App',
    data() {
      return {
        users: JSON.stringify([{ name: "John Wick" }, { name: "IronMan" }])
      }
    }
  }
</script>

<style>
	#app {
		font-family: Avenir, Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
		margin-top: 60px;
	}
</style>