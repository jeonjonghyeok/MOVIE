<h3> ▶ 프로젝트명   :</h3> All in movie 
<h3> ▶ 개발 환경    :</h3> 
<li> OS 및 DB : Windows7, MySQL</li>
  <li> 사용 Tool : Eclipse</li>
<li> 프로그래밍 언어 : JAVA, Servlet, JSP</li>
<li> 웹표준 기술 : HTML, CSS, Javascript, jQuery</li>
<li> 프레임워크 : Spring, MyBatis</li>
<h3>▶ 인    원     :</h3> 5명 
<h3>▶ OS 및 DB     :</h3> Window 10, MySQL 
<h3>▶ 사용 언어    :</h3> JAVA 
<h3>▶ 프로젝트 소개 :</h3><p>All in movie란 CGV, 롯데 시네마, 메가박스 대표적인 영화3사의 서비스를 통합하여 제공하는 서비스를 말합니다. 영화를 보고 싶은 시간에 맞춰 예매 하는 경우 맞는 시간대를 찾아 3사의 상영관정보를 각각 확인하여 비교해야 하는 불편함이 있습니다. All in movie는 이러한 불편한 점을 해결하고자 3사에서 제공하는 상영 정보들을 통합하여 사용자에게 제공하는 서비스를 말합니다. </p>

<h3>▶ 본인 역할    :</h3> <p>프로젝트 진행 시에 로그인, 회원가입, DB구현, 예매 기능을 담당 </p>
1. DB:
<p>영화관 서비스에 대한 정보를 분석하여 eXERD 도구를 이용하여 개체(회원, 게시판, 예약, 상영 시간표, 상영관, 영화, 극장)를 생성하고, 영화, 예약, 상영관을 상영시간표를 통해 서로 연결하였습니다. 이후 데이터 표현방법을 정의한 데이터 명명 규칙에 맞춰 설계하고 설계된 ERD를 바탕으로 DDL, DML문을 이용하여 MySQL에서 테이블을 생성하고 데이터를 추가하였습니다. 하지만 프로그램 개발을 진행하면서 ERD의 수정이 반복적으로 있었기 때문에 즉각 반영하여 테이블을 반복적으로 수정했습니다.</p>
2. 회원가입, 로그인
<p>MVC모델 방식을 사용하여 회원가입 view의 Form을 통해 입력 받은 사용자의 ID, 이름, 주민번호, 전화번호, 이메일, 암호를 MemberVO 객체를 생성하면서 입력 받은 정보를 초기화 하여 이후 Mapper에서 xml파일로 정의한 쿼리문을 이용하여 MemberVO객체의 정보를 Mysql의 Client테이블에 저장하였습니다.
로그인 사용자로부터 입력 받은 id와 password 값을 MemberVO객체를 생성하면서 초기화 시키고, MySQL로부터 id에 해당하는 password값을 불러와 두 값을 비교하고 Password가 일치하면 사용자에 대한 세션을 생성하고 로그인 성공, Password가 일치하지 않거나, 아이디가 존재하지 않을 경우 예외 처리 경고문을 통해 사용자가 바로 알 수 있도록 하였습니다.</p>
3. 예매
<p>영화에 대한 정보(영화제목, 시간, 감독, 배우, 관람 기준, 개봉일)가 저장되어 있는 MOVIE 테이블의 튜플들을 미리 저장한 이미지와 함께 매핑시켜 홈페이지에 출력하고 출력된 영화 이미지를 클릭하면 해당 영화의 예매 화면으로 이동하게 하였습니다.
영화 선택-> 날짜 선택-> 지역 선택-> 극장 선택-> 시간 선택 -> 좌석 선택 순으로 예매할 수 있도록 개발하였습니다.</p>
test readme
