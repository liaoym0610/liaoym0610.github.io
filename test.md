<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>flex布局</title>
	<style>
		body{
			background-color: #874C92;
			display: flex;
			flex-wrap: wrap;
		}
		.box{
			background-color: #fff;
			border-radius: 10px;
			width:104px;
			height: 104px;
			padding:4px;
			margin:10px;
		}
		.item{
			background-color: #000;
			width:24px;
			height:24px;
			border-radius: 24px;
			margin:4px;
		}
		.p100{
			display: flex;
		}
		.p101{
			display: flex;
			justify-content: center;
		}
		.p102{
			display: flex;
			justify-content: flex-end;
		}
		.p110{
			display: flex;
			align-items: center;
		}
		.p111 {
		  display: flex;
		  justify-content: center;
		  align-items: center;
		}
		.p121 {
		  display: flex;
		  justify-content: center;
		  align-items: flex-end;
		}
		.p122 {
		  display: flex;
		  justify-content: flex-end;
		  align-items: flex-end;
		}

		.p2_00_02 {
		  display: flex;
  		  justify-content: space-between;
		}
		.p2_00_20 {
		  display: flex;
  		  justify-content: space-between;
  		  flex-direction: column;
		}
		.p2_01_21 {
		  display: flex;
  		  justify-content: space-between;
  		  flex-direction: column;
  		  align-items: center;
		}
		.p2_02_22 {
		  display: flex;
  		  justify-content: space-between;
  		  flex-direction: column;
  		  align-items: flex-end;
		}
		.p2_00_11{
			display: flex;
		}
		.p2_00_11 .item:nth-child(2){
			align-self: center;
		}
		.p2_00_22 {
		  display: flex;
		  justify-content: space-between;
		}
		.p2_00_22 .item:nth-child(2) {
		  align-self: flex-end;
		}

		.p3_00_11_22 {
		  display: flex;
		}
		.p3_00_11_22 .item:nth-child(2) {
		  align-self: center;
		}
		.p3_00_11_22 .item:nth-child(3) {
		  align-self: flex-end;
		}


		.p4_00_01_02_22 {
		  display: flex;
		  flex-wrap: wrap;
		  justify-content: flex-end;
		  align-content: space-between;
		}
		.p4_00_02_20_22 {
		  display: flex;
		  flex-wrap: wrap;
		  align-content: space-between;
		}
		.p4_00_02_20_22 .column {
		  flex-basis: 100%;
		  display: flex;
		  justify-content: space-between;
		}

		.p6_1 {
		  display: flex;
		  flex-wrap: wrap;
		  align-content: space-between;
		}
		.p6_2 {
		  display: flex;
		  flex-direction: column;
		  flex-wrap: wrap;
		  align-content: space-between;
		}
		.p6_3 {
		  display: flex;
		  flex-wrap: wrap;
		}
		.p6_3 .row{
		  flex-basis: 100%;
		  display:flex;
		}
		.p6_3 .row:nth-child(2){
		  justify-content: center;
		}
		.p6_3 .row:nth-child(3){
		  justify-content: space-between;
		}

		.p9 {
		  display: flex;
		  flex-wrap: wrap;
		}
	</style>
</head>
<body>
<h1><a href="http://www.ruanyifeng.com/blog/2015/07/flex-examples.html">flex布局教程</a></h1>
<!-- 1个项目 -->
<div class="box p100">
  <span class="item"></span>
</div>
<div class="box p101">
  <span class="item"></span>
</div>
<div class="box p102">
  <span class="item"></span>
</div>
<div class="box p110">
  <span class="item"></span>
</div>
<div class="box p111">
  <span class="item"></span>
</div>
<div class="box p121">
  <span class="item"></span>
</div>
<div class="box p122">
  <span class="item"></span>
</div>
<!-- 2个项目 -->
<div class="box p2_00_02">
  <span class="item"></span>
  <span class="item"></span>
</div>
<div class="box p2_00_20">
  <span class="item"></span>
  <span class="item"></span>
</div>
<div class="box p2_01_21">
  <span class="item"></span>
  <span class="item"></span>
</div>
<div class="box p2_02_22">
  <span class="item"></span>
  <span class="item"></span>
</div>
<div class="box p2_00_11">
  <span class="item"></span>
  <span class="item"></span>
</div>
<div class="box p2_00_22">
  <span class="item"></span>
  <span class="item"></span>
</div>
<!-- 3个项目 -->
<div class="box p3_00_11_22">
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
</div>
<!-- 4个项目 -->
<div class="box p4_00_01_02_22">
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
</div>
<div class="box p4_00_02_20_22">
  <div class="column">
    <span class="item"></span>
    <span class="item"></span>
  </div>
  <div class="column">
    <span class="item"></span>
    <span class="item"></span>
  </div>
</div>
<!-- 6个项目 -->
<div class="box p6_1">
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
</div>
<div class="box p6_2">
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
</div>
<div class="box p6_3">
  <div class="row">
    <span class="item"></span>
    <span class="item"></span>
    <span class="item"></span>
  </div>
  <div class="row">
    <span class="item"></span>
  </div>
  <div class="row">
     <span class="item"></span>
     <span class="item"></span>
  </div>
</div>

<!-- 9个项目 -->
<div class="box p9">
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
  <span class="item"></span>
</div>


</body>
</html>
