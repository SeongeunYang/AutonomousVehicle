<h3 align="center"><b>📰 (교내) 자율주행 ECP 해커톤 경진대회 / 대상 📰</b></h3>
<h4 align="center">📆 2021.01 ~ 2021.02</h4>
<br>

---

<img src="https://user-images.githubusercontent.com/57797592/152646238-511fae04-be62-46ab-ab8c-26443bb9cd71.png" />
<h3><b>🎫 프로젝트 소개 🎫</b></h3>
소형 보드(Jetson Nano)를 이용한 자율 주행 모형차 제작 및 개발

<br>
<h3><b>👨🏻‍🤝‍👨🏻 Members 👨🏻‍🤝‍👨🏻</b></h3>
팀장 : 양성은
<br>팀원 : 손형섭, 원해연, 김하림, 이수영, 박유나, 고동현

---

<h3><b>🛠 Tech Stack 🛠</b></h3>
<p>
<img src="https://img.shields.io/badge/JetsonNano-FC5230?style=for-the-badge&logo=JetsonNano&logoColor=white">
<img src="https://img.shields.io/badge/C-ED8B00?style=for-the-badge&logo=C&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-1F497D?style=for-the-badge&logo=Python&logoColor=white">
</p>

---

<h3><b>1️⃣ 시스템 기능블록도</b></h3>
<img src="https://user-images.githubusercontent.com/57797592/152645931-c0e06ca0-c686-4967-aaa7-ee95223fcdb3.png" />

<br><br>
<h3><b>2️⃣ 전체 시스템 구성</b></h3>
<img src="https://user-images.githubusercontent.com/57797592/152645959-9710cd76-5e65-4b85-b54f-7375a6128a69.png" />

<br><br>
<h3><b>🏷 주요 기능 🏷</b></h3>
<h4><b>📰 Cartographer SLAM을 이용한 지도 Mapping 📰</b></h4>
<table width="100%">
    <tr>
        <td width="50%"><img src="https://user-images.githubusercontent.com/57797592/152646607-e7110654-dd29-42a6-9213-81f2d2905807.gif" /></td>
        <td width="50%">
            <ul>
                <li>구글 사에서 제공하는 오픈 소스 SLAM을 꾸준한 업데이트와 정보가 올라오고 있다.<br>- 반면 다른 SLAM 방식(Ex. Gmapping) 같은 경우 16년도에 업데이트를 중단하여 오래되었다.</li>
                <li>독립형 C++ 라이브러리이며 ROS를 제공하여 기존의 ROS 시스템과 연결성이 좋다.</li>
                <li>로컬에서 직접 연산을 하는 다른 SLAM들과 달리 백엔드가 존재하여 연산 속도가 비교적 빠르다.</li>
            </ul>
        </td>
    </tr>
</table>

<br>
<h4><b>📰 ROS를 이용한 자율 주행 시스템 📰</b></h4>
<table width="100%">
    <tr>
        <td width="50%"><img src="https://user-images.githubusercontent.com/57797592/152646948-40930219-fddf-431e-be9f-283b566a8d14.png" /></td>
        <td width="50%">
            <ul>
                <li>Mapping된 지도 데이터와 Lidar를 통한 경로 탐색 기능</li>
                <li>VESC를 이용한 모터 제어로 주행 및 방향 전환 기능</li>
            </ul>
        </td>
    </tr>
	  <tr>
        <td width="50%"><img src="https://user-images.githubusercontent.com/57797592/152646709-a277df72-b8f5-4aa3-9258-687498e9cdfb.gif" /></td>
        <td width="50%">
            <ul>
                <li>IMU센서를 이용한 미끄러짐 발생 시 긴급 정지 기능</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td width="50%"><img src="https://user-images.githubusercontent.com/57797592/152646673-8826ba4f-6b98-416c-a287-8bff47a4cb24.gif" /></td>
        <td width="50%">
            <ul>
                <li>Ultra Sonic 센서를 이용한 장애물 감지 시 일시 정지 기능(장애물이 사라지면 다시 주행을 시작함)</li>
            </ul>
        </td>
    </tr>
	  <tr>
        <td width="50%"><img src="https://user-images.githubusercontent.com/57797592/152646771-b27bac96-428c-4ae7-b869-05ed4601448e.gif" /></td>
        <td width="50%">
            <ul>
                <li>Steering Angle(바퀴 회전 각도)에 따라 코너 구간 판단 후 코너 구간 감속</li>
            </ul>
        </td>
    </tr>
</table>

<h4><b>📰 인벤터를 활용한 차량 프레임 3D 도면 설계, 3D 프린팅으로 프레임 완성 📰</b></h4>
<table width="100%">
    <tr>
        <td width="50%"><img src="https://user-images.githubusercontent.com/57797592/152647038-74fc0582-1c10-4dd1-b530-b4f355642c78.png" /></td>
        <td width="50%"><img src="https://user-images.githubusercontent.com/57797592/152647018-d4def209-c050-4263-a38d-0dca395a1ebc.png" /></td>
    </tr>
</table>
<br>

---

<h3 align="center"><b>✏ Trouble Shooting ✏</b></h3>
<br>
<details>
    <summary>
        <b>SLAM 방식의 변경</b>
    </summary>
    <br>자세히 보기 : https://indecisive-viscount-244.notion.site/Cartographer-SLAM-7a1b7dfd51bf46389a185ce661fec740
</details>
