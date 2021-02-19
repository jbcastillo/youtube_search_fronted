<template>
	<v-app id=" app">

		<v-app-bar
			:clipped-left="$vuetify.breakpoint.lgAndUp"
			app
			color="blue darken-3"
			dark
		>
			<img width="50" height="50" src="@/assets/youtube-icon.svg" />

			<v-toolbar-title style="width: 300px" class="ml-0 pl-4">
				<span
					style="font-family: 'Gill Sans Extrabold', Helvetica, sans-serif;"
					class="hidden-sm-and-down"
				>
					Youtube Search
				</span>
			</v-toolbar-title>
		</v-app-bar>
		<v-main>
			<v-slide-y-transition mode="out-in">
				<router-view />
			</v-slide-y-transition>
		</v-main>

		<v-footer 
			dark 
			padless 
			app
			:clipped-left="$vuetify.breakpoint.lgAndUp"
		>
			<v-card color="primary" class="flex" flat tile>
				<v-card-text class="py-2 white--text text-center">
					Jesus Castillo {{ new Date().getFullYear() }}
				</v-card-text>
			</v-card>
		</v-footer>
	</v-app>
</template>

<script>


export default {
	name: "App",
	data() {
		return {
		};
	},
	computed: {
	},
	created() {

	},
	methods: {
	},
};
</script>

