<!-- 
  Messenger:

  Displays given messages for warning, error, and success
 -->
<template>
	<div class="messenger">
		<div class="box-bar small warn" v-show="messages.warn">
			<span><i class="fa fa-exclamation-triangle fa-fw dashicon warn" aria-hidden="true"></i> {{ messages.warn }}</span></div>
		<div class="box-bar small error" v-show="messages.error">
			<span><i class="fa fa-times-circle fa-fw" aria-hidden="true"></i> {{ messages.error }}</span></div>
		<div class="box-bar small success" v-show="messages.success">
			<span><i class="fa fa-check fa-fw" aria-hidden="true"></i> {{ messages.success }}</span></div>
	</div>
</template>

<script>
	export default {
		props: {
			messages: Object
		}
	}
</script>

<style lang="scss">
	@import "../styles/settings.scss";
</style>