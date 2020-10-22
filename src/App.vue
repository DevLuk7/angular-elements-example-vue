<template>
	<users-list :userslist="users" @userselect="userselect"></users-list>;
</template>

<script>
	export default {
    name: 'App',
    data() {
      return {
        users: JSON.stringify([{ name: "John Wick" }, { name: "IronMan" }])
      }
    },
    methods: {
      userselect(event) {
        alert(event)
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