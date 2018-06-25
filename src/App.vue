<template>
	<v-app>
		<v-navigation-drawer v-model="sideNav" app fixed clipped>
			<v-list>
				<v-list-tile @click="">
					<v-list-tile-action>
						<v-icon>supervisor_account</v-icon>
					</v-list-tile-action>
					<v-list-tile-content>
						<v-list-tile-title>View Meetups</v-list-tile-title>
						
					</v-list-tile-content>
				</v-list-tile>
			</v-list>
		</v-navigation-drawer>
		<v-toolbar app fixed clipped-left>
			<v-toolbar-side-icon @click.stop="sideNav = !sideNav"
			class="hidden-sm-and-up">
			</v-toolbar-side-icon>
			<v-toolbar-title>
				DevMeetup
			</v-toolbar-title>
			<v-spacer></v-spacer>
			<v-toolbar-items class="hidden-xs-only">
				<v-btn flat>
					<v-icon left>
						supervisor_account
					</v-icon>
					View Meetups
				</v-btn>
			</v-toolbar-items>
		</v-toolbar>
		<main>

		</main>
	</v-app>
	</template>

<script>
export default {
  data () {
    return {
      sideNav: false
    }
  },
  name: 'App'
}
</script>
<style lang="stylus">
  @import '~vuetify/src/stylus/main'
</style>