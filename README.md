# 2022-hackathon
### 팀명
- 나띵벗(Nothing But)
----------

### 제출 세션 및 주제
- 특별세션 - 일회용품, 재활용 쓰레기
----------

### 프로젝트 한 줄 설명
- 텀블러를 통해 탄소중립을 실천하는 카페들을 소개하는 프로젝트
----------
### 프로젝트에 대한 설명 : 
- **슬로건** : Bring Your Own Tumble

- **문제점** : 잦은 일회용품 컵, 빨대 사용등으로 인한 하루에 발생하는 약 53만톤의 폐기물, 환경오염 및 쓰레기 처리비용 증가

- **‘Tumble’ 프로젝트 소개** : 텀블러를 가지고갈 경우 음료 할인을 받을 수 있는 카페를 리스트업해서 사용자에게 제공해줍니다.
일상속에 가장 작은 행동으로써 탄소중립을 실천하고 일회용품 배출량을 줄임으로써 지구를 구할 수 있습니다.

- **서비스 타겟층** :
평소 환경 및 탄소중립에 관심이 많거나 새로운 캠페인에 관심이 많은 사용자들이 주요 타겟층, 하지만 환경에 관심이 없어도 텀블러로 인한 혜택을 받고싶은 일반 사용자들을 타겟으로 합니다.


- **주요기능** : 
Tumble 서비스의 로그인/회원가입 및 로그아웃
Tumble 을 소개할수있는 켐페인 소개
지도와 리스트를 통한 텀블러 사용시 혜택을 주는 카페소개
Tumble 사용자들의 카페방문후기 및 편하게 이야기 나눌수 있는 Tumble 만의 커뮤니티

- **기대효과** : 
재활용을 하는 것이 환경을 지키는 방법이 아닌, 자신의 텀블러를 사용함으로써 일회용품의 사용을 줄이게 된다면 폐기물의 수를 급격하게 줄일 수 있을 것입니다.
텀블러 사용 시 혜택을 주는 카페를 소개함으로써 홍보 효과와 동시에 홍보를 위한 카페 점주들의 Tumble 수요도 증가하게 될 것으로 기대됩니다.

----------
### 프로젝트에 활용된 기술(3가지 이내)
- Front-End : JavaScript, Thymeleaf, Bootstrap
- Back-End : Spring Boot, Jpa, MariaDB on Amazon RDS
- ETC : Kakao 지도 Web API

> > - **Spring Boot**
> > > > 1. Http Session세션을 사용해서 로그인에 성공하면 session 속성에 유저 정보를 저장할 수 있습니다.
> > > > 2. 웹 브라우저를 완전히 종료하기전까지 session객체 정보를 사용해 로그인상태를 계속해서 유지할 수 있습니다.
> > > > 3. session.invalidate() 메서드를 통해 로그아웃 처리를 할 수 있습니다.
> > > > 4. 회원 / 비회원 권한 구별 ---> **회원만 접근 가능한 기능** : 글작성, 수정, 삭제, 마이페이지
> > > > 5. 조회수 기능 - Entity 내의 Board 클래스안에 viewCount 의 변수를 만들어 각 Board 객체의 viewCount 를 DB와 연동되어 조회시에 Count+1 이 됩니다


> > - **Jpa**
> > > > 1. 검색 기능 - JPA 기본제공 함수인 FindBy 함수를 사용해 FindBy(Title)Containing 함수를 통해 제목 검색 기능을 구현했습니다. 
> > > >  ex ) “가나다” 에 가나다를 검색해야 나오는것이 아닌 중간글자인 “나”를 검색하게 되면 “나”가 포홤된 모든 글들의 검색결과가 나오게 됩니다.
> > > > 2. 글 작성 기능 - JPA 기본제공 함수인 Save 함수를 사용하여 글 작성 기능을 구현하였습니다. 글을 작성하게 되면 사용자 ID, 글 작성일자가 Setting 되어 작성되게 됩니다.
> > > > 3. 글 삭제 기능 - JPA 기본제공함수인 DeleteById 를 사용하여 글 삭제 기능을 구현하였습니다. 글 번호에 따라 글이 삭제 되게 구현하였습니다.

> > - **Kakao 지도 Web API**
> > > > 1. 석환

----------
### 시연 영상
