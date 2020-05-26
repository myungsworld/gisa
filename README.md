## gisa

#### 소프트웨어 생명 주기
폭포수,프로토타입,나선형,애자일    
    
---
|구분|폭포수|애자일|
|:---:|:---:|:---:|
새로운 요구사항 반영|어려움|지속적으로 반영
고객과의 의사소통|적음|지속적임
테스트|마지막에 모든 기능 테스트|반복되는 일정 주기 끝날때마다 테스트
개발중심|계획,문서|고객   

---
#### 스크럼 기법   
제품책임자(PO)-사용자,개발의뢰자로써 백로그작성    
스크럼마스터     
개발팀  
#### 스크럼 개발 프로세스    
제품 백로그 작성->스프린트 계획회의->스프린트(개발)->일일스크럼 회의->스프린트 검토 회의->스프린트 회고

---
#### XP기법
짧은 개발주기를 반복해 요구사항 적극 반영하는 것  
XP의 핵심 가치 5-의단용존피(의사소통,단순성,용기,존중,피드백)  
#### XP기법 프로세스
사용자 스토리->릴리즈 계획수립->스파이크->이터레이션->승인검사->소규모 릴리즈  
__릴리즈__-부분적으로 기능이 완료된 제품을 제공  
__이터레이션__-릴리즈를 더 세분화 한 단위  
__승인 검사__-고객이 직접 수행하고 다음 이터레이션 진행  

---
#### 요구사항 정의
__요구분석 단계__  
타당성조사->추출및분석->명세화->검증  
__요구사항 분석 기법__  
분개할협정(요구사항 분류,개념 모델링,할당,협상,정형 분석)  
__요구사항 확인 기법__  
검프검인(검토,프로토타입,검증,인수테스트)  
~~분석기법과 확인기법 구분가능해야함~~  
__시스템 요구사항 분석 절차__  
요구사항 선별->요구사항 분류->관련자료준비->분석 및 명세서 구체화->명세서 공유  
__인터페이스 요구사항 검토 방법__  
__워크스루__:1~2시간 짧은 검토  

---
#### UML(모델링언어)
__사물__  
구행그주(구조,행동,그룹,주석)  
__다이어그램__
정적-구조적 다이어그램,동적-행위 다이어그램
구현단계 다이어그램(배치,컴포넌트)  
__관계__
의존= 점선화살표  
일반화= 실선세모
포함= 검은마름모  
집합= 하얀마름모  
실체화 =점선세모

---
#### 사용자 인터페이스
__CLI(Command Line Interface)__:명령과 출력이 텍스트 형태로 이뤄지는 인터페이스  
__GUI(Graphic User Interface)__:아이콘이나 메뉴를 마우스로 선택하여 작업을 수행하는 그래픽 환경의 인터페이스  
__NUI(Natural User Interface)__:사용자의 말이나 행동으로 기기를 조작하는 인터페이스  

---
#### UI 설계도구
__와이어프레임__:기획 초기에 제작,페이지에 대한 개략적인 레이아웃이나 UI 요소 뼈대 설계 단계(스케치,일러스트)  
__스토리보드__:와이어프레임에 __디스크립션__(화면에 대한 설명,전반적인 로직 설명)을 추가한것(파워포인트,Axure)  
__프로토타입__:와이어프레임이나 스토리보드에 __인터랙션__(상호작용 표현)추가 한것 __동적__인 형태의 모형(HTML/CSS)  
__목업__:와이어프레임보다 좀 더 실제화면처럼 만든 __정적__ 형태의 모형  
__유스케이스__:내가 암  

---
#### 품질 요구사항
__ISO/IEC 9126__ 표준: 신사기이유효(신뢰성,사용성,기능성,이식성,유지 보수성,효율성)  
__기능성__:사용자의 요구사항을 정확하게 만족하는 기능을 제공하는지 여부  
__신뢰성__(__가용성__):__오류__ 없이 수행할수 있는 정도  
__사용성__:향후 다시 사용하고 싶은 정도  
__효율성__:할당된 시간동안 한정된 자원으로 얼마나 빨리 처리하는 정도  
__유지 보수성__:다른 환경에서 __개선__ , __확장__ 하는 정도  
__이식성__:다른 환경에서도 얼마나 쉽게 __적용__ 하는지 정도  

---
#### UI
__인터랙션__: UI를 통해 시스템과 작용하는 일련이 상호작용 EX)마우스로 화면을 클릭하면 화면이 반응  
__인터랙션__ 은 __UI__ 시나리오 중 작성  
__GUI__ 는 __UI__ 시나리오 다음 작성  

---
#### 소프트웨어 아키텍쳐
__기본원리__:추모단정(추상화,모듈화,단계적 분해,정보 은닉)  
- __아기텍쳐패턴__  
    1. __레이어패턴__:상위계층이 하위계층으로 서비스 제공(OSI참조모델)  
    1. __클라이언트 서버 패턴__:  
    1. __파이프 필터 패턴__:스트림절차로 컴포넌트로 캡슐화하여 파이프 통해 데이터 전송(UNIX SHELL)  
    1. __모델 뷰 컨트롤러 패턴__:  
    1. __마스터 슬레이브 패턴__:장애 허용시스템과 병렬컴퓨팅  
    1. __브로커 패턴__:분산 환경 시스템  
    1. __피어 투 피어 패턴__:멀티스레딩  
    1. __이벤트 버스 패턴__:  
    1. __인터프리터 패턴__:프로그램 코드의 각 라인을 수행하는 방법 지정 컴포넌트 설계  

---
#### 모듈
__응집도__:__하나__ 의 모듈을 구성하는 요소 관의 관계  
__결합도__:__두개__ 의 모듈을 구성하는 요소 관의 관계  
    - __응집도__ 가 강한 순서 : 기순교절시논우(기능,순차,교환,절차,시간,논리,우연)  
    - __결합도__ 가 강한 순서 : 내공외제쓰자(내용,공통,외부,제어,스탬프,자료)  
        1. 스탬프 결합도:__자료구조__ 라는 말이 들어가면 됨  
        2.  
__공통모듈 명세기법__:명완일추정(명확,완정,일관,추정,정확)  
__인터페이스 요구사항 검증 주요 항목__:명완일추검변(명확,완전,일관,추적가능,검증가능,변경용이)  

---
#### 코드
코드의 주요기능:__식분배(식별,분배,배열)__  
|코드종류|순차코드|블록코드|10진코드|그룹분류코드|연상코드|표의 숫자코드|합성코드|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|예시|1,2,3,4|1001~1100:총무부|1000:공학|1-01-001:본사-총무부-인사계|TV-40:40인치TV|120-720-1500:두께폭길이|KE-711:대한항공 711기|

---
#### 인터페이스
__인터페이스 송수신방법 명세화__:발통처연(발생주기,통신유형,처리유형,연계방식)  
__인터페이스 통신 유형__:단방향,동기,비동기  
__시스템 인터페이스 설계서__=인터페이스 식별 및 명세 기술

---
#### 미들웨어
__DB__:DB를 사용해 시스템 구축하는 경우 2티어 아키텍쳐  
__RPC__(원격 프로시저 호출):Entera,ONC/RPC  
__MOM__(메시지 지향 미들웨어):비동기형 메세지 전달 방식 미들웨어  
__TP-Monitor__(트랜잭션 프로세싱 모니터):항공기나 철도예약 같은 온라인 트랜잭션 처리 및 감시  
__ORB__(객체요청브로커):객체지향 미들웨어 __코바__(CORBA) 표준 스펙 구현한 미들웨어  

---
#### 자료구조
__비선형구조__:트리,그래프  
__선형리스트__:
|선형리스트|연속리스트|연결리스트|
|:---:|:---:|:---:|
|구조|배열|포인터|
|효율|좋음|별로|
|속도|빠름|느림|
|자료의 이동|어려움|용이|


---
#### 데이터베이스
__DBMS(주요기능)__: 정의,조작,제어  
제어:무결성,권한검사,병행제어  
__데이터 무결성__:데이터를 보호 및 유지 데이터의 변조,방지를 위한 모든 과정          

---
#### SQL
__절차형 SQL__  
|프로시저|사용자 정의 함수|
|:---:|:---:|
|SELECT, WHERE, HAVING 절에 프로시저를 사용할 수 없음|SELECT, WHERE, HAVING 절에 사용자 정의 함수를 사용할 수 있음|
|반환값 여러개이거나 반환하지 않음|반환값이 return|
|프로시저안에 프로시저 호출가능|사용자 정의 함수 안에 프로시저 호출 불가|
0

개념적 설계- 트랜잭션(원자성,고립성(격리성),일관성,지속성)    
논리적 설계- DBMS
물리적 설계- 접근 경로,방법,응답시간,저장공간의 효율화

비트맵 인덱스-데이터종류가 적고 동일한 데이터가 많은 경우(분포도가 낮은경우) 최적의 성능을 발휘
인덱스와 테이블 데이터는 분리하여 설계

속성들이 가질수잇는 모든값들의 집합=도메인
같은 개체를 갖는 속성들의 집합=개체

predicate calculus - 관계해석 

테이블스페이스-논리적인 영역
데이터 파일-물리적인 영역

원자성-All of nothing 전부가 아니면 아무것도 아니다

클러스터 -동일한 성격의 데이터를 동일한 데이터 블록에 저장하는 물리적 저장 방법 조회속도 빠르게되지만 입력 수정 삭제는 느리게 됨
        -단일 테이블 클러스터링->처리 범위 넓은경우
        -다중 ->조인이 많은 경우

        
파티션 대용량 테이블,인덱스를 논리적인 단위로 나누는 것
       local partioned index 1:1 대응 이게 데이터 관리 더 쉬움
       global partitioned index 독립적 
       범위 분할->데이터가 집중되는 단점 발생
       해쉬 분할->데이터를 분산하여 분할
분산데이터의 위치 투명성은 독립적이다,
            사이트간의 오류발생률은 높지만 그 기능이 계속 수행될순 있다
            데이터는 일관성있어야 한다 가용성 높여야한다 

접근통제 3요소 - 정보커 (정책,보안모델,메커니즘)
                보안모델-정형모델
                메커니즘-기술적 방법
                정책-신분기반,규칙기반,역할기반
#### 보안    
인가된 사용자가  접근-> 기밀성        
수정-> 무결성(인가된 사용자만 데이터 수정할수 있게하는 것)    
                        
데이터베이스 백업 로그파일-시간의흐름에따라 기록한 파일 (작업순서x)

스토리지 -DAS 직접연결되서 속도는 빠르지만 다른서버에서 접근불가
        -NAS 네트워크를 통해 연결 서버들이 자유롭게 접근 서버가 증가하면?
        -SAN 위에둘 짬뽕 파이버채널(FC)하면 SAN

슈퍼타입테이블->하나
서브타입테이블->여러개 1:1관계임 두개
두개가 하나로 통합된 테이블에는 모든 서브타입 속성을 포함해야됨

준거성=표준성

SQL예약어는 될수있으면 컬럼명으로 사용하지 않아야한다.
한개의insert 명령어로는 하나의 테이블만 생성가능
한개의 DELET 문에는 한개의 테이블만 사용가능
SQL에서 조건문= WHERE,LIKE
절차형 sql은 모듈화가 가능하다

integer 4바이트 정수
smalliant 2바이트 정수
float 부동 소수점 수
decimal 10진 소수

table의 check절은 인덱스에 대한 정보를 저장

프로시저에서 EXCEPTION은 BEGIN-END 영역안에서 오류발생한 경우 처리

DELETE는 테이블에서 튜플삭제
DROP은 프로시져,트리거
<>은 같지않다를 의미함

트리거의 구문에는 DCL을 사용할수 없다
EVENT 트리거가 실행되는 조건을 명시 (트리거에만 있음)

프로시저는 IN OUT이 다 있고 사용자 정의 함수는 IN만 있다 IN은 전달받고 OUT은 반환하는것
사용자 정의함수는 다른 사용자정의함수를 호출가능,프로시저 호출불가

Dynamic SQL은 SQL을 자유롭게 변경할수 있어 NULL을 처리하는 함수 사용할 필요가 없다
WEB server -> WAS -> DBMS

ORM -재사용과 유지보수가 쉽다 ,객체가 데이터베이스에 독립적,SQL은 학습해야함

MYSQL 사용자 권한 확인 SQL문 SHOW GRANTS FOR 사용자@호스트(URL)

데이터 전환 ,데이터 전환 계획서
데이터 정제요청서의 정제 방법에는 원천,전환,모두가 있다

소프트웨어 개발환경 하드웨어는 클라이언트와 서버로 구성된다.
                    소프트웨어 개봘환경은 개발도구(개발환경 ex.Eclipse)들로 구성된다. 도구와 관련없는것들(HTML 웹만듬 요런거)

개발언어의 선정기준:적정성,효율성,이식성,친밀성,범용성

웹서버는 정적, WAS는 동적 서비스 제공

프레임워크의 특성 :모듈화,재사용성,확장성,제어의 역흐름

배치 프로그램의 수행주기 :정기,이벤트성,ON-DEMAND 배치

사용자와 상호작용 없이 작업들이 미리 정해진 순서에 따라 일괄적으로 처리되는것 : batch program

quartz(배치 스케줄러): 위치 시간 추적 가능

c언어 문자는 작은따옴표,문자열은 큰따옴표
c언어에서 사용하는 기억클래스:register auto static extern
반복문은 3가지 while for do (if 아님) 문장구조 성격
%x=16진수
%d=10진수
%o=8진수
%u=부호없는 10진수

%8.5s=전체 8자리 확보하여 5자리만 출력
%2.1f=소수점한자리까지 출력 그뒤에껀 반올림
%-7d=왼쪽에 붙여서 출력하려면 - 를  
c언어는 기계어가 아니다 컴파일러 언어이다,시스템 프로그래밍에 적합한 언어이다.,unix 운영체제이다

a & b = a와b를 2진수로 나타내어서 AND연산한 
a l b = OR 연산
a ^ b = NOR 연산

1+X<<2 = 더하기를 먼저한후 << 실행 X=3이면 16이 나옴

switch(a):a는 실수형은 불가능

서버용 스크립트 언어:ASP,JSP,PHP
클라이언트용 스크립트 언어:자바 스크립트

폰노이만구조-명령형언어
함수형언어=적용형언어
논리형언어-선언형언어

getchar,putchar함수는 서식열문자를 사용할수없음 %d 이런거

운영체제는 하드웨어 위 4계층에 위치
windows- 싱글유저 멀티테스킹
unix- 멀티유저 멀티테스킹

unix-트리구조,c언어,대화식,높은 이식성과 호환성
     백그라운드 장점:다중작업이 가능함
     쉘:명령어 해석기,파이프라인 기능 담당,사용자와 시스템간의 인터페이스 제공
     커널:아무고토안함

주기억장치 -반입(fetch):프로그램을 주기억장치로 가져오는 시기를 결정
           -배치(placement)
           -재배치(replacement)
           
고정 분할 할당과 동적 분할 할당으로 나누어 관리되는 기법:연속 로딩 기법

페이징-내부 단편화
세크멘테이션-외부 단편화 발생
인위적 연속성은 가상에서는 인위적으로 연속적일 필요가 없다는 것

LRU - 가장 오랫동안 사용되지 않았던 것
하드웨어 비트가 필요한 기법-NUR (호출0변형0비트가 제일빠르고 1 1 이 제일 느리게 교체된다)

시간구역성-루프,스택,부 프로그램,COUNTING,집계
공간구역성은 위에꺼 제외한 나머지

페이지들의 집합-위킹 셋
선점스케쥴링 종류-RR(round Robin),SRT,다단계 큐

프로토콜 기본요소 -의구타 의미,구문,타이밍
ARP - 논리->물리 RARP 그반대
RTCP는 하상 32의비트의 경계로 끝난다

페이지크기가 클수록 전체적인 입출력 효율이 증가된다.

비용산정기법

비용결정요소3가지-프자생(프로젝트,자원,생산성)
프로젝트요소-제시요(제품복잡도,시스템크기,요구되는신뢰도)
자원요소-인하소(인적,하드웨어,소프트웨어)
생산성요소-개발자 능력,개발 기간

하향식-여러전문가의 경험 바탕,비과학적
     의 전문가 감정 기법-전문가 두명이서 하는거 (주관 뚜렷)
     의 델파이-한명의 조정자 ,여려 전문가 (주관 방지)
상향식-세부적인 단위 비용 산정후 전체 비용 산정
     의 LOC 기법 (원시코드 라인수,SOURCE OF LINE)-노력(인월):개발기간,투입 인원
     
### 소프트웨어 추정모형   
COCOMO-LOC기법    
      의 분류 조직형,반분리형,내장형(차례대로 5만 라인 이하, 30만 이하 , 30만 이상)    
      의 종류 기본형,중간형,발전형
Putnam-
      의 SLIM
FP(기능점수)
      의 ESTIMACS

소프트웨어의 생명주기-기본,지원,조직
프로젝트 관리의 유형-일비인위품(보안은 없음) 일정비용인력위험품질

#### 소프트웨어 개발표준
SPICE의 수행능력 단계- 불완전->수행->관리->확립->예측->최적화    
CMMI의 역량 성숙도 평가(Capability Maturity Integration Model)    
    의 프로세스 성숙도- 초기->관리->정의->정략적관리->최적화
ISO/IEC 12207    
    
#### 소프트웨어 개발방법론
테일러링의 내부적요건-목요프보    
        의 외부적요건-법표    
        의 기법 4가지-규모와복잡도,프로젝트 구성원,팀내 방법론 지원,자동화    
    
#### 경로제어프로토콜(ROUTING PROTOCOL)    
IGP-내부(RIP-소규모 OSPF-대규모)
EGP-외부(BGP는 EGP단점보안)    
    
흐름제어의 정지및대기-한 번에 하나의 프레임 전송   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
        의 슬라이딩윈도우-한 번에 여러개의 프레임 전송    
    
소프트웨어 개발보안 관련 주체-감사한(KISA)발행    

#### 암호 알고리즘    
1.블록 암호화    
-           의 SEED-한국진흥원-128비트,키 길이 128,256    
-           의 ARIA-산학연합회-128비트,키 길이 가변

2.개인키 암호화    
-            의 DES알고리즘-블록크기 64비트,키 길이 56비트    
-            의 AES알고리즘-블록크기 128비트,키 길ㅇ이 가변(128,192,256)
3.공개키 암호화    
-            의 RSA알고리즘
-            의 DSA알고리즘

