<!-- index.vue -->
<template>
  <view>
	<view><!-- 放首页的图片 -->
		<image class="logo" src="/static/logo.png"></image>
	</view>
	
	<div class="inputPhoneNum"><!-- 输入手机号框-->
		<image src="/static/phoneNum.png" class="logo01"></image>
		<input type="text" placeholder="请输入手机号" class="numBox">
	</div>
	
	<div class="inputPhoneNum"><!--输入密码框-->
		<image src="/static/password.png" class="logo01"></image>
		<input type="text" placeholder="请输入密码" class="numBox">
	</div>
	
	<view class="forgetPassword"><!--忘记密码模块-->
		<navigator url="/pages/retrievePasswordPage/retrievePasswordPage">
			<text>忘记密码</text>
		</navigator>
	</view>
	
	<view class="positionButton"><!--登录按钮-->
		<button size="mini" class="loginButton">登录</button>
	</view>
	
	<view class="logonBox"><!--无账号注册模块-->
		<text>没有账号？</text>
		<navigator url="/pages/registerPage/registerPage" hover-class="navigator-hover">
			<text style="color: #11d183;">注册</text>
		</navigator>
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
.forgetPassword{
	margin-top: 30px;
	margin-left: 40px;
}

//登录按钮
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

//"注册"盒子
.logonBox{
	margin-top: 40px;
	display: flex;
	justify-content: center;
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
	margin-top: 40px;
}
</style>