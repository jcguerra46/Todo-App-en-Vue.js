<template>
	<div>
		<div v-if="remaining == 1">{{ remaining }} tarea pendiente</div>
		<div v-else-if="remaining == 0">Tareas terminadas</div>
		<div v-else>{{ remaining }} tareas pendientes</div>
	</div>
</template>

<script>
	export default {
		name: 'todo-remaining',
		props: {
			remaining: {
				type: Number,
				required: true,
			}
		}
	}
</script>