<template>
  <div class="android_controls">
			<div class="controls_inner">
				<div><img src="../assets/images/android/back.png"></div>
				<div><img src="../assets/images/android/menu.png"></div>
				<div><img src="../assets/images/android/tab.png"></div>
			</div>
	</div>
</template>
<script>

</script>
<style>
.android_controls{
  width: 100%;
  height: 70px;
  position: absolute;
  bottom: 0;
  left: 0;
  background-color: black;
}
.controls_inner{
	width: 70%;
	height: 100%;
	display: block;
	margin: 0 auto;
}

.controls_inner div{
	width: 33.3333333%;
	height: 100%;
	display: flex;
	align-items: center;
	justify-content: center;
	float: left;
}

.controls_inner div img{
	width: 25px;
}
</style>
