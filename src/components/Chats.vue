<template>
  <div class="messages_section dragscroll">

			<div class="single_chat">
				<div class="image_container">
					<img src="../assets/images/chats/chat2.jpg">
				</div>

				<div class="content_container">
					<div class="content_container_inner">
						<p class="user_name"><name>Harry</name> <span>1:45 AM</span></p>
						<p class="chat_content">Hello my name is Harry and I... <span>1</span></p>
					</div>
				</div>
			</div>

			<div class="single_chat">
				<div class="image_container">
					<img src="../assets/images/chats/chat3.jpg">
				</div>

				<div class="content_container">
					<div class="content_container_inner">
						<p class="user_name"><name>Ellie</name> <span>11:21 AM</span></p>
						<p class="chat_content">Sorry I didn't see your message ar...<span>1</span></p>
					</div>
				</div>
			</div>

			<div class="single_chat">
				<div class="image_container">
					<img src="../assets/images/chats/chat4.jpg">
				</div>

				<div class="content_container">
					<div class="content_container_inner">
						<p class="user_name"><name>Alfie</name> <span>7:23 AM</span></p>
						<p class="chat_content">Hey did you catch the game lastni... <span>3</span></p>
					</div>
				</div>
			</div>

			<div class="single_chat">
				<div class="image_container">
					<img src="../assets/images/chats/chat6.jpg">
				</div>

				<div class="content_container">
					<div class="content_container_inner">
						<p class="user_name"><name>Charlie</name> <span class="read">TUESDAY</span></p>
						<p class="chat_content">Don't forget my charger from your hous..</p>
					</div>
				</div>
			</div>

			<div class="single_chat">
				<div class="image_container">
					<img src="../assets/images/chats/chat7.jpg">
				</div>

				<div class="content_container">
					<div class="content_container_inner">
						<p class="user_name"><name>Xing</name> <span class="read">TUESDAY</span></p>
						<p class="chat_content">Did I leave my laptop at your house on...</p>
					</div>
				</div>
			</div>

			<div class="single_chat">
				<div class="image_container">
					<img src="../assets/images/chats/chat8.jpg">
				</div>

				<div class="content_container">
					<div class="content_container_inner">
						<p class="user_name"><name>Martin</name> <span class="read">MONDAY</span></p>
						<p class="chat_content">I guess hahaha so when are yo...</p>
					</div>
				</div>
			</div>
		</div>
</template>
<script>
  export default {


  }
</script>
<style>
.messages_section{
	width: 100%;
	height: calc(100% - 80px);
	box-sizing: border-box;
	padding-bottom: 49px;
	background-color: white;
	overflow: hidden;
}

.content_container{
	width: calc(100% - 80px);
	display: flex;
	align-items: center;
	height: 100%;
}

.content_container_inner{
	height: auto;
	float: left;
	margin-left: 20px;
	box-sizing: border-box;
	width: 100%;
}

.single_chat{
	width: 100%;
	height: 110px;
	position: relative;
	box-sizing: border-box;
	padding: 10px 30px;
}

.image_container{
	height: 100%;
	display: flex;
	width: 80px;
	align-items: center;
	justify-content: center;
	float: left;
}

.user_name{
	font-family: 'Helvetica Neue Bold';
	color: black;
	font-size: 22px;
	width: 100%;
	display: block;
	letter-spacing: 1.1px;
}

.image_container img{
	height: 90%;
	border-radius: 999px;
}

.chat_content{
	width: 100%;
	display: block;
	font-family: 'Helvetica Neue Light';
	font-size: 20px;
	color: rgba(165, 165, 165, 0.8);
}

.chat_content span{
	background-color: #00d260;
	float: right;
	border-radius: 999px;
	padding: 5px;
	box-sizing: border-box;
	width: 30px;
	overflow: hidden;
	height: 30px;
	text-align: center;
	color: white;
	font-family: 'Helvetica Neue Bold';
	font-size: 18px;
	vertical-align: -3px;
	line-height: 19px;
}

.user_name span,
.read{
	color: #00d260;
	font-family: 'Helvetica Neue Medium';
	font-size: 16px;
	float: right;
}

.read{
	color: rgba(165, 165, 165, 0.8) !important;
}

.single_chat:hover{
	cursor: pointer;
	background-color: rgba(165, 165, 165, 0.2);
}

.single_chat:after{
	width: 50%;
	height: 1px;
	content: "";
	background-color: rgba(165, 165, 165, 0.8);
	left: 50%;
	transform: translate(-50%, 0);
	position: absolute;
	bottom: 0;
}


</style>
