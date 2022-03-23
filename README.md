# vibrating-heart
Vibrating and animated heart shape with color text using html and css.

<!DOCTYPE html>
<html>
<head>
	<title>CSS Heart Shape</title>
	<link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
	<div id="main">

	<h1 style="color: red">I</h1><br><br>

	<div class="heart"></div><br><br>
	
	<h1 style="color: red">YOU</h1>
    <p>India</p>
	<style >
	p{
		color:red;
		font-size:50px;
	}

body{
	margin: 0;
	padding: 0;
	min-height: 100vh;
	display: flex;
	align-items: center;
	justify-content: center;
	background: #0b1522;
}
.heart{
	height: 70px;
	width: 70px;
	background: #f20044;
	position: relative;
	transform: rotate(-45deg);
	box-shadow: -10px 10px 90px #f20044;
	animation: heart 0.6s linear infinite;
}
@keyframes heart{
	0%{
			transform: rotate(-45deg) scale(1.07);
	}
	80%{
			transform: rotate(-45deg) scale(1.0);
	}
	100%{
			transform: rotate(-45deg) scale(1.07);
	}
}
.heart:before{
	content: '';
	position: absolute;
	height: 70px;
	width: 70px;
	background: #f20044;
	top: -50%;
	border-radius: 50px;
	box-shadow: -10px -10px 90px #f20044;
}

.heart:After{
	content: '';
	position: absolute;
	height: 70px;
	width: 70px;
	background: #f20044;
	right: -50%;
	border-radius: 50px;
	box-shadow: 10px 10px 90px #f20044;
}
</style>
</body>
</html>
