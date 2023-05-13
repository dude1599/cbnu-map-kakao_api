# Cbnu-kakao-map-api
사용자가 원하는 장소의 위도와 경도만 알면 카카오 지도 API를 통해 입력한 장소의 카카오 지도를 볼 수 있게 해주는 시스템
This is a code that displays Chungbuk National University on the web using the Kakao Maps API.

#project name : CBNU kakao map

#project execution period : 2023-04 ~ 2023-05

## Description
Cbnu-kaka-map-api는 kakao map api를 사용하여 사용자가 원하는 장소의 위도와 경도를 소스에 입력 시 입력한 좌표의 장소를 일상적으로 우리가 사용하는
카카오 맵 형식으로 웹에서 볼 수 있게 해주는 프로젝트입니다.

본인의 로컬 호스트 서버를 열어서 (ex:http:localhost~/파일이름.html) 본인이 입력한 좌표를 카카오 맵 형식으로 볼 수 있습니다.


#최종 결과창
![2023-05-13](https://github.com/dude1599/cbnu-map-kakao_api/assets/133233495/66befae9-95da-42ea-a4bc-ce3010537617)



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
