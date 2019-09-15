<!DOCTYPE html>
<html>
<head>
	<title>월급계산기</title>
</head>

<style type="text/css">
		body {width: 1200px;display: block;margin:auto;}
		.header{font-weight: bold;width: 1200px; background: #92679F;opacity: 0.77;display: block;height: 120px;font-size: 36px;text-align: center;margin-top:0px;padding-top: 70px;color:white;}
		#sec {width:270px;display: block;font-size: 20px;text-align: left;padding-top: 100px;padding-bottom: 100px;margin: auto;}
		.footer{width:1200px; background: #92679F;opacity: 0.77; height: 50px;color:white;font-size: 12px;display: block;text-align: center;padding-top: 7px;}
		
</style>


<body>
	<section class ="header">월급계산기
	</section>

 	<div id="sec">
	 	<input type="checkbox" id="under15" value="15">주 15시간 이하

		<br><input type="text" id="time" placeholder="한달동안 총 근무시간을 입력하세요">

		<input type="button" value="확인" id="ok">

		<div id="monitor">당신의 월급은 000원입니다.</div>


		<script type="text/javascript">
			ok.onclick = function (){			
				var smoney = (time.value*8350);
				monitor.innerHTML = "당신의 원급은" + Math.round(smoney) + "원입니다";}
		</script>

	<br><br><br>

	  <input type="checkbox" id="up15" value="15"> 주 15시간 이상

		<br><input type="text2" id="ttime" placeholder="한달동안 총 근무시간을 입력하세요">
		<br><input type="text3" id="date" placeholder="한주동안 근무일을 입력하세요">
		<input type="button" value="확인" id="ok2">

		<div id="monitor2">당신의 월급은 000원입니다.</div>

		<script type="text/javascript">
			ok2.onclick = function (){		
				var extra = ttime.value/date.value;
				var smoney = (ttime.value*8350 + extra*8350);
				monitor2.innerHTML = "당신의 원급은" + Math.round(smoney) + "원입니다";}
		</script>
		</div>
		
	<div class="footer">
		<p> copyright&copy;2019 한경대학교 정미소. 모든 권리 보유</p>
	</div>
</body>
</html>
