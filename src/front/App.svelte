<script>
	import Router from "svelte-spa-router";
	import ContacstTable from './ContactsTable.svelte';
	import Home from './Home.svelte';
	import EditContact from "./EditContact.svelte";

	const routes ={

		"/": Home,
		"/contactList": ContacstTable,
		"/contact/:contactName": EditContact
	};

</script>

<main>
	<h1>Contact Manager</h1>
	<Router {routes} />

	
</main>

<style>
	h1 {
		color: red;
	}
</style>

