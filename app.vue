<template>
	<NuxtLayout>
		<NuxtLoadingIndicator />
		<NuxtPage />
	</NuxtLayout>
</template>

<style>
	.layout-enter-active,
	.layout-leave-active {
		opacity: 1;
		transition: opacity 0.2s ease-in-out;
	}
	.layout-enter-from,
	.layout-leave-to {
		opacity: 0;
	}
</style>
