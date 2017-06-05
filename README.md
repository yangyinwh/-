# -<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>心跳</title>
	<!-- 
		
	 -->
	<style type="text/css">
		/* 动画效果 */
		/* 跳动效果 */
		@keyframes bigger{
			from{}
			to{
				transform:scale(1.5, 1.5) rotateZ(45deg);
				/* transform:scale(1.3, 1.3); */
			}
		}

		/* 阴影效果 */
		@keyframes shadow{
			from{}
			to{
				box-shadow: 0px 0px 60px pink;
			}

		}
			body{
				background-color:black;
			}

		.heart{
			width: 300px;
			height: 300px;
			margin:200px auto;
			/* border:1px solid #0094ff; */
			position:relative;
			/* 添加动画效果 让整颗心 动起来  */
			animation: bigger 1s infinite alternate;
		}
		.heart div{
			width: 200px;
			height: 200px;
			background-color:pink;
			position:absolute;
			/* 添加阴影的动画 */
			animation: shadow 1s infinite alternate;
			/* animation: bigger 1s infinite alternate; */
		}
		.cycle{
			border-radius:50%;
		}
		.right{
			right:0px;
		}
		.bottom{
			bottom: 29px;
			left:50px;
			transform: rotateZ(45deg) scale(.85, .85);
			
		}

		.heartMan{
			top:20px;
			left:50px;
			transform: scale(.85, .85);
			background:url('img/wyz.jpg') center/200px 200px;
		}
	</style>
</head>
<body>
	<div class="heart">
		<div class="left cycle"></div>
		<div class="right cycle"></div>
		<div class="bottom"></div>
		<div class="heartMan"></div>
	</div>
</body>
</html>
