<!-- index.vue -->
<template>
  <view>
	<navigator url="/pages/index/index">
	<view><!-- 放首页的图片 -->
		<image src="/static/backButton.png" class="backButtonPosition"></image>
		<image class="logo" src="/static/logo.png"></image>
	</view>
	</navigator>
	
	<div class="inputPhoneNum"><!-- 输入手机号框-->
		<image src="/static/phoneNum.png" class="logo01"></image>
		<input type="text" placeholder="请输入手机号" class="numBox">
	</div>
	
	<div class="inputPhoneNum"><!--重新设置密码框-->
		<image src="/static/password.png" class="logo01"></image>
		<input type="text" placeholder="请重新设置密码" class="numBox">
	</div>

	<div class="inputPhoneNum"><!--输入验证码框-->
		<image src="/static/verificationLogo.png" class="logo01"></image>
		<input type="text" placeholder="请输入验证码" class="numBox">
		<button class="verificationButton">验证码</button>
	</div>
	
	<view class="positionButton"><!--登录按钮-->
		<button size="mini" class="loginButton">注册</button>
	</view>
	
	<view class="otherLogonBox"><!--“其他登录方式”+“微信跳转图标”模块-->
		<view>
			<text>------其他登录方式------</text>
		</view>
		
		<view>
			<image src="/static/Logo_WeChat.png" class="Logonlogo"></image>
		</view>
	</view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      
    };
  },
};
</script>

<style>
//头部Logo设计
.logo{
	width: 390px;
	height: 270px;
}
//输入手机号或是密码框
.logo01{
	width: 40px;
	height: 40px;
	margin-right: 10px;
	margin-left: 10px;
}
.inputPhoneNum{
	display: flex;
	align-items: center;
	margin-top: 40px;
}
//"忘记密码"盒子
.numBox{
	font-size: 22px;
	border-bottom: 2px solid black;
	padding-bottom: 6px;
}


//注册按钮
.loginButton{
	font-size: 20px;
	color: black;
	background-color: #d8f1f2;
}
.positionButton{
	margin-top: 35px;
	display: flex; /* 使用flex布局 */  
	justify-content: center; /* 水平居中 */  
	align-items: center; /* 垂直居中 */ 
}


//其他登录方式模块
.Logonlogo{
	width: 50px;
	height: 50px;
	display: block;
}
.otherLogonBox{
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	margin-top: 60px;
}

//验证码按钮
.verificationButton{
	width: 100px;
	font-size: 20px;
	color: black;
	background-color: #d8f1f2;
}

.backButtonPosition{
	position: absolute;
	top: 0px;
	left: 0px;
	z-index: 1;
	
	//按钮样式
	width: 40px;
	height: 40px;
}
</style>