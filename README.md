# cbnu-kakao-map-api
This is a code that displays Chungbuk National University on the web using the Kakao Maps API.

#최종 결과창
![cbnu kakao map](https://github.com/dude1599/cbnu-map-kakao_api/assets/133233495/37897c92-7609-41a2-a2cb-85fd9e8eeea7)

# Source Code
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8"/>
	<title>처음 Kakao 지도 시작하기</title>
</head>
<body>
    <div>
        <h2>
            [오픈소스 기초프로젝트 HW #1] - 2020037001 이희윤 <충북대학교 위치 카카오 맵을 통해 나타내보기>
        </h2>
       
    </div>
    <div>
        <h1>안녕하세요 이희윤입니다. 이젠 충북대학교를 찍어보겠습니다.</h1>
        <h3> 충북대학교 위도: 36.6291° N / 경도: 127.4568° E</h3>
    </div>
    
	<div id="map" style="width:500px;height:400px;"></div>
	<script type="text/javascript" src="//dapi.kakao.com/v2/maps/sdk.js?appkey=c744ae648c6c2389a5dd006b130d2027"></script>
	<script>
		var container = document.getElementById('map');
		var options = {
			center: new kakao.maps.LatLng(36.6291, 127.4568),   // 지도중심의 위도&경도 좌표
			level: 3           // 지도 확대 수치. 기존 : 3, 변경 후 : 6
		};

		var map = new kakao.maps.Map(container, options);
	</script>
</body>
</html>
