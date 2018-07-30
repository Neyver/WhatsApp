<template>
<div class="body">
  <div class="container">

	<!-- Dropdown Menu -->
	<div class="dropdown_menu">
		<p class="dropdown_item">New group</p>
		<p class="dropdown_item">New broadcast</p>
		<p class="dropdown_item">WhatsApp Web</p>
		<p class="dropdown_item">Starred Messages</p>
		<p class="dropdown_item">Settings</p>
	</div>

	<!-- Search Bar -->
	<div class="back_trigger"></div>
	<input type="text" class="search_bar">

	<!-- Lightbox -->
	<div class="lightbox">
		<div class="lightbox_container">
			<h1 class="lightbox_name">Marc</h1>

			<div class="lightbox_image">
				<img src="images/chats/chat2.jpg">
			</div>

			<div class="lightbox_controls">
				<div class="one_control"><img src="images/icons/chat.png"></div>
				<div class="one_control"><img src="images/icons/phone.png"></div>
				<div class="one_control"><img src="images/icons/video.png"></div>
				<div class="one_control"><img src="images/icons/info.png"></div>
			</div>
		</div>
	</div>

		<div class="title_bar">
			<div class="title_top">
				<div class="title_container">
					<p>WhatsApp</p>
				</div>

				<div class="icon_container">
          <div><img src="./assets/images/menu.png"></div>
          <div class="icon_container_search"><img src="./assets/images/search.png"></div>
				</div>
			</div>

			<div class="tab_menu">
				<p class="single_tab active">CHATS</p>
				<p class="single_tab">STATUS</p>
				<p class="single_tab">CALLS</p>
			</div>
		</div>
    <Chats/>
    <Foot/>
</div>
</div>
</template>

<script>
import Chats from './components/Chats.vue';
import Foot from './components/Foot.vue';
export default {
  name: 'App',
  components: {
    Chats,
    Foot
  }
}
</script>

<style>
*{
	margin: 0;
	padding: 0;
	list-style: none;
	text-decoration: none;
	-webkit-touch-callout: none;
	-webkit-user-select: none;
	-khtml-user-select: none;
	-moz-user-select: none;
	-ms-user-select: none;
	user-select: none
}
.body {
  background-image: url(./assets/images/background.jpg);
	background-size: cover;
	background-position: center;
	background-repeat: no-repeat;
}

.container{
	width: 506px;
	height: 900px;
	display: block;
	box-sizing: border-box;
	overflow: hidden;
	border-top: solid 35px #054d44;
	background-color: black;
	margin: 50px auto;
	position: relative;

}

.dropdown_menu{
	width: 0px;
	height: 0px;
	overflow: hidden;
	background-color: white;
	box-shadow: 0px 0px 4px rgba(165, 165, 165, 0.5);
	position: absolute;
	right: 5px;
	top: 5px;
	z-index: 999;
}

.dropdown_item{
	width: 100%;
	font-family: 'Helvetica Neue Light';
	box-sizing: border-box;
	padding: 12px 20px;
	background-color: white;
}

.lightbox{
	width: 506px;
	height: 900px;
	z-index: 99999999;
	top: 50px;
	opacity: 0;
	align-items: center;
	justify-content: center;
	position: fixed;
	background-color: rgba(16, 16, 16, 0.6);
	display: none;
}

.back_trigger{
	width: 34px;
	height: 39px;
	background-color: transparent;
	position: absolute;
	display: none;
	left: 20px;
	top: 10px;
	cursor: pointer;
	z-index: 999;
}

.search_bar{
	width: 100%;
	position: absolute;
	height: 60px;
	box-shadow: -1px -10px 13px 10px #101010;
	border: none;
	font-family: 'Helvetica Neue Light';
	font-size: 24px;
	color: #101010;
	text-decoration: underline;
	padding: 0px 10px 0px 70px;
	background-image: url(./assets/images/icons/back.png);
	background-position: 22px 17px;
	background-size: 30px 24px;
	display: none;
	opacity: 0;
	background-repeat: no-repeat;
}

.lightbox_container{
	width: 340px;
	height: 400px;
	background-color: white;
	position: relative;
	display: none;
}

.lightbox_name{
	width: 100%;
	position: absolute;
	top: 0;
	box-sizing: border-box;
	letter-spacing: 1.1px;
	left: 0;
	padding: 7px 7px;
	font-family: 'Helvetica Neue Light';
	font-size: 22px;
	color: white;
	background-color: rgba(16, 16, 16, 0.5);
}

.lightbox_image{
	width: 100%;
	height: 340px;
}

.lightbox_image img{
	width: 100%;
	height: 100%;
}

.icon_container div:nth-child(1){
	width: 10px;
}

.lightbox_controls{
	width: 100%;
	height: 60px;
	background-color: white;
}

.one_control{
	width: 25%;
	height: 100%;
	float: left;
	display: flex;
	align-items: center;
	justify-content: center;
}

.one_control img{
	width: 30px;
}

.title_bar{
	background-color: #075e54;
	width: 100%;
	height: 150px;
}

.title_top{
	overflow: hidden;
	width: 90%;
	display: block;
	margin: 0 auto;
	height: 90px;
}

.title_container{
	height: 100%;
	width: 50%;
	display: flex;
	align-items: center;
	float: left;
}

.title_container p {
	font-family: 'Helvetica Neue Light';
	color: white;
	letter-spacing: 2px;
	font-weight: 600;
	font-size: 26px;
}

.icon_container{
	width: 30%;
	float: right;
	height: 100%;
}

.icon_container img{
	height: 30px;
	cursor: pointer;
}

.icon_container div{
	height: 100%;
	display: flex;
	width: 100px;
	align-items: center;
	justify-content: center;
	float: right;
}

.tab_menu{
	width: 100%;
	overflow: hidden;
	height: 60px;
}

.single_tab{
	width: 33.333333333333333333%;
	height: 100%;
	display: flex;
	align-items: center;
	justify-content: center;
	box-sizing: border-box;
	float: left;
	font-family: 'Helvetica Neue Medium';
	letter-spacing: 1.3px;
	font-weight: 600;
	font-size: 18px;
	border-bottom: solid 3px transparent;
	color: rgba(165, 165, 165, 0.8);
}

.single_tab:hover,
.active{
	color: white;
	border-color: white;
	cursor: pointer;
}


</style>
