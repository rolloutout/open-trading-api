#### **[당사에서 제공하는 샘플코드에 대한 유의사항]** ####
- 샘플 코드는 한국투자증권 오픈API(KIS Develpers)를 연동하는 예시입니다. 고객님의 개발부담을 줄이고자 참고용으로 제공되고 있습니다.
- 샘플 코드는 별도의 공지 없이 지속적으로 업데이트될 수 있습니다.
- 샘플 코드를 활용하여 제작한 고객님의 프로그램으로 인한 손해에 대해서는 당사에서 책임지지 않습니다.

![header](https://capsule-render.vercel.app/api?type=waving&color=gradient&height=300&section=header&text=한국투자증권%20KIS%20Developers&fontSize=50&animation=fadeIn&fontAlignY=38&desc=Open%20Trading%20API%20Docs&descAlignY=51&descAlign=62)

## 1. KIS Developers 개발자 센터 소개
[KIS Developers](https://apiportal.koreainvestment.com/)는 한국투자증권의 트레이딩 서비스를 오픈API로 제공하여 개발자들이 다양한 금융서비스를 만들 수 있도록 지원하는 개발자 센터입니다. KIS Developers에서는 개발자의 금융 서비스 개발을 지원하기 위해 API 문서 메뉴 내 API에 대한 상세한 설명과 예제를 제공합니다. 전문 개발자가 아닌 일반인들도 쉽게 금융 서비스를 만들 수 있습니다.

* 제휴 문의는 [제휴안내 페이지](https://apiportal.koreainvestment.com/howto-register)에서 제휴 신청 부탁드립니다.
* API 사용 관련 문의는 [Q&A 페이지](https://apiportal.koreainvestment.com/community/10000000-0000-0011-0000-000000000003)에서 문의 부탁드립니다.


## 2. 이용 안내
### 2.1. 사전 준비
KIS Developers 서비스 신청을 위해서는 2가지 사전 준비물이 필요합니다. 첫 번째로는 한국투자증권 계좌가 개설되어있어야 하며, 두 번째로는 한국투자증권 ID 등록이 필요합니다. 만약 계좌가 없으시다면 한국투자증권 앱을 통해 비대면 개설을 진행하거나, 가까운 영업점을 방문해주시길 바랍니다. (모의투자계좌의 경우, 한국투자 홈페이지 혹은 MTS에서 모의투자 서비스 신청 후 발급받은 모의계좌번호로 API 신청을 하셔야 합니다.)

-   한국투자증권 앱 :  [https://securities.koreainvestment.com/main/customer/cusGuide/customerGuide.jsp](https://securities.koreainvestment.com/main/customer/cusGuide/customerGuide.jsp)
-   가까운 영업점 찾기 :  [https://securities.koreainvestment.com/main/customer/guide/branch/branch.jsp](https://securities.koreainvestment.com/main/customer/guide/branch/branch.jsp)
-   모의투자계좌 발급 : [https://securities.koreainvestment.com/main/research/virtual/_static/TF07da010000.jsp](https://securities.koreainvestment.com/main/research/virtual/_static/TF07da010000.jsp)


### 2.2. 서비스 신청

KIS Developers 서비스 신청 페이지까지 2가지 경로로 접속 가능합니다.

* KIS Developers 우상단 API신청 버튼 클릭
* 한국투자증권 홈페이지 [서비스신청 > Open API > KIS Developers > KIS Developers 서비스 신청하기]

서비스 신청 화면에 접속하면 홈페이지 인증서 로그인 화면이 뜨고, 인증을 완료하면 아래와 같이 KIS Developers 서비스 신청하기의 첫 화면인 휴대폰 인증 화면이 뜨게 됩니다.

![](https://wikidocs.net/images/page/159301/kis_restapi_1.png)

해당 화면에서 등록하신 휴대폰 인증을 통해 본인 인증을 완료합니다.

* HTS ID에 $나 @가 포함되면 추후에 HTS ID 변경 시 Open API 서비스 사용에 제한이 있을 수 있으니, HTS ID 변경 후 서비스 가입을 권유드립니다. 
* 다만 기존 가입내역이 있으며 HTS ID 변경 후 Open API 서비스 사용에 어려움을 겪으실 경우, KIS Developers 홈페이지 Q&A 게시판에 문의 남겨주시면 조치해 드리겠습니다.

### 2.3. 유의사항 확인
![image](https://github.com/koreainvestment/open-trading-api/assets/87407853/9413332d-105c-47aa-89de-7d419714a0fb)

다음으로는 유의사항확인입니다. 서비스 사용에 관한 유의사항을 정독하여 충분하게 숙지하신 뒤, 동의를 진행합니다. 개인정보 수집·이용 동의서, 고객 이용약관 및 이용약관 개정 알림에 대해 미동의 시, 서비스 이용이 불가합니다.



### 2.4. KIS Developers 서비스 신청하기
![](https://wikidocs.net/images/page/159301/kis_restapi_3.png)

유의사항 확인이 완료되면 기존 신청내역이 없으실 경우, 곧바로 서비스 신청하기 팝업 화면이 뜨게 됩니다. 해당 화면에서 보유하고 계신 계좌에 대하여 API 신청하실 수 있습니다. 한 번에 2개의 계좌까지 API 신청 가능하며, 다계좌 API 신청을 원하실 경우, 신청하기 완료 후 신청정보 페이지에서 추가신청하기 기능을 이용하시기 바랍니다.

* 실전투자계좌의 경우 동일한 종합 계좌번호의 주식(국내, 해외), 선물/옵션 계좌로 API 이용 가능합니다.
* 모의투자계좌의 경우 한국투자 홈페이지 혹은 MTS에서 모의투자 서비스 신청 후 발급받은 모의계좌번호로 API 신청을 하셔야 합니다.

계좌번호 선택 하단에 위치한 테이블에 있는 KIS Developers 사용자 ID는 향후 KIS Developers 포탈에서 사용되는 ID로 기존 등록된 HTS ID와 동일합니다. 두번째로 API그룹은 현재 KIS Developers에서 이용 가능한 API 기능들로, 지속적으로 추가 개발될 예정입니다. 세번째로 문자메시지 설정을 통해 서비스 만료 1개월 전 메시지를 받을 수 있으니 참고하시길 바랍니다. 마지막으로 이용기간은 신청일로부터 1년입니다. 

계좌번호를 선택 혹은 입력하시고 신청 버튼을 누르시면 처음 홈페이지 로그인하신 방식으로 인증 팝업이 뜨게 됩니다. 

![](https://wikidocs.net/images/page/159301/kis_restapi_6.png)

정상적으로 인증을 완료하였다는 메시지가 창에 뜨고, 해당 계좌번호로 API 신청 및 APP Key, APP Secret 발급이 완료됩니다.

![](https://wikidocs.net/images/page/159301/kis_restapi_4.png)

이상으로 신청이 완료되었습니다. 카카오톡 알림톡 혹은 문자 메시지로 오픈API 서비스 신청완료 안내 메시지와 함께 KIS Developers 홈페이지 초기 패스워드가 발송됩니다. KIS Developers 홈페이지의 ID는 HTS ID와 같으며, 메시지로 받으신 임시비밀번호로 홈페이지에 로그인하셔서 API문서 등을 확인하실 수 있습니다.


### 2.5. 신청정보

![](https://wikidocs.net/images/page/159301/kis_restapi_7.png)

신청이 완료되면 신청정보 화면의 신청현황 테이블에서 해당 계좌의 App Key와 App Secret을 확인하실 수 있습니다. App Key와 App Secret은 노출되어 있지 않아, 클립보드에 복사 후 원하시는 곳에 붙여넣어 사용 부탁드립니다. App Key와 App Secret 두 암호키를 통해 계좌에 접근할 수 있는 토큰을 발급받을 수 있어, 타인에게 유출을 금하며 관리에 유의해야합니다. 유출시 즉시 홈페이지에서 재발급 하시기 바랍니다.

갱신 기능과 해지 기능에 대해 설명드리겠습니다. 갱신(기간 연장)은 만료 30일 전부터 신청 가능하며, 그 전까지는 갱신 버튼이 비활성화되어 클릭이 불가능합니다. 갱신 시, 신청일로부터 1년 기간이 연장되며, APP Key, APP Secret가 재발급됩니다. 해지는 언제든지 신청 가능하며, 해지 완료 시 발급되었던 APP Key, APP Secret는 사용이 불가능합니다.


### 2.6. 추가신청하기

![](https://wikidocs.net/images/page/159301/kis_restapi_5.png)

신청현황 화면 하단의 추가신청하기 기능을 이용하여 더 많은 계좌의 API 신청이 가능합니다. 실전투자계좌의 경우 최대 89개, 모의투자계좌의 경우 최대 2개까지 신청 가능합니다. 추가 신청 프로세스는 맨 처음 신청했을 때와 동일하게 계좌 선택 및 비밀번호 인증, 인증서 인증을 거쳐 이뤄집니다.

### 2.7. 초기 로그인 시 패스워드 변경 방법
오픈API 서비스 신청 완료 후 KIS Developers 포탈로 이동하여 로그인을 진행합니다. 초기 아이디는 HTS 아이디와 동일하며, 홈페이지 신청 정보를 통해 확인하실 수 있습니다. 초기 패스워드는 안내 메시지 카카오톡 알림톡 혹은 문자 메시지로 발송됩니다. 반드시 로그인 후 패스워드를 변경하시길 바랍니다. 패스워드 변경은 아래와 같이 진행하실 수 있습니다.

**■ 초기 로그인 시 패스워드 변경 방법**
![image](https://github.com/koreainvestment/open-trading-api/assets/87407853/3a8c0973-eb43-469c-a95d-eac7878c54bb)
![image](https://github.com/koreainvestment/open-trading-api/assets/87407853/5e99326d-fb09-4b24-8678-7ef9e69fbd7f)


### 2.8. 이전 ID 신청정보 삭제 방법 

KIS Developers 서비스 가입 후 HTS ID를 변경하여 '처리계좌의 ID와 사용자정보가 상이하여 주문처리 불가능 합니다.' 오류가 발생하셨을 경우 아래와 같이 한국투자증권 홈페이지에서 이전 ID 신청정보 삭제하신 후 핸드폰 인증 후 신청현황에서 신청을 다시 하시고 발급받으신 앱키를 이용하시면 정상 이용하실 수 있습니다.

**■ 이전 ID 신청정보 삭제 방법**
![image](https://github.com/koreainvestment/open-trading-api/assets/87407853/c331efc3-0c5c-4722-8e69-3c50924a73b4)
한국투자증권 홈페이지 > 트레이딩 > Open API > KIS Developers > KIS Developers 서비스 신청하기 접속 후 'ID 변경 전 신청정보 삭제' 클릭
(https://securities.koreainvestment.com/main/customer/systemdown/RestAPIService.jsp) 
  
## 3. API 제공 목록 <a id="apiList">

|구분 |API명 |모의투자 제공 여부|
|--|--|--|
|OAuth인증|웹소켓접속키발급|⭕|
|OAuth인증|접근토큰발급|⭕|
|OAuth인증|접근토큰폐기|⭕|
|OAuth인증|Hashkey|⭕|
|[국내주식]주문/계좌|주식주문(현금)|⭕|
|[국내주식]주문/계좌|주식주문(신용)| |
|[국내주식]주문/계좌|주식주문(정정취소)|⭕|
|[국내주식]주문/계좌|주식정정취소가능주문조회| |
|[국내주식]주문/계좌|주식일별주문체결조회|⭕|
|[국내주식]주문/계좌|주식잔고조회|⭕|
|[국내주식]주문/계좌|매수가능조회|⭕|
|[국내주식]주문/계좌|주식예약주문| |
|[국내주식]주문/계좌|주식예약주문정정취소| |
|[국내주식]주문/계좌|주식예약주문조회| |
|[국내주식]주문/계좌|퇴직연금 체결기준잔고| |
|[국내주식]주문/계좌|퇴직연금 미체결내역| |
|[국내주식]주문/계좌|퇴직연금 매수가능조회| |
|[국내주식]주문/계좌|퇴직연금 예수금조회| |
|[국내주식]주문/계좌|퇴직연금 잔고조회| |
|[국내주식]주문/계좌|주식잔고조회_실현손익| |
|[국내주식]주문/계좌|신용매수가능조회| |
|[국내주식]주문/계좌|투자계좌자산현황조회| |
|[국내주식]주문/계좌|기간별매매손익현황조회| |
|[국내주식]주문/계좌|기간별손익일별합산조회| |
|[국내주식]주문/계좌|매도가능수량조회| |
|[국내주식]기본시세|주식현재가 시세|⭕|
|[국내주식]기본시세|주식현재가 체결|⭕|
|[국내주식]기본시세|주식현재가 일자별|⭕|
|[국내주식]기본시세|주식현재가 호가 예상체결|⭕|
|[국내주식]기본시세|주식현재가 투자자|⭕|
|[국내주식]기본시세|주식현재가 회원사|⭕|
|[국내주식]기본시세|국내주식기간별시세(일/주/월/년)|⭕|
|[국내주식]기본시세|주식현재가 당일시간대별체결|⭕|
|[국내주식]기본시세|주식현재가 시간외일자별주가|⭕|
|[국내주식]기본시세|주식당일분봉조회|⭕|
|[국내주식]기본시세|주식현재가 시세2| |
|[국내주식]기본시세|ETF/ETN 현재가| |
|[국내주식]기본시세|NAV 비교추이(종목)| |
|[국내주식]기본시세|NAV 비교추이(분)| |
|[국내주식]기본시세|NAV 비교추이(일)| |
|[국내주식]기본시세|국내주식 장마감 예상체결가| |
|[국내주식]기본시세|ETF 구성종목시세| |
|[국내주식]기본시세|국내주식 시간외현재가| |
|[국내주식]기본시세|국내주식 시간외호가| |
|[국내주식]ELW시세|ELW현재가 시세|⭕|
|[국내주식]ELW시세|ELW 상승률순위| |
|[국내주식]ELW시세|ELW 거래량순위| |
|[국내주식]ELW시세|ELW 지표순위| |
|[국내주식]ELW시세|ELW 민감도 순위| |
|[국내주식]ELW시세|ELW 당일급변종목| |
|[국내주식]ELW시세|ELW 신규상장종목| |
|[국내주식]ELW시세|ELW 투자지표추이(체결)| |
|[국내주식]ELW시세|ELW 투자지표추이(분별)| |
|[국내주식]ELW시세|ELW 투자지표추이(일별)| |
|[국내주식]ELW시세|ELW 변동성 추이(틱)| |
|[국내주식]ELW시세|ELW 변동성 추이(체결)| |
|[국내주식]ELW시세|ELW 변동성 추이(분별)| |
|[국내주식]ELW시세|ELW 변동성 추이(일별)| |
|[국내주식]ELW시세|ELW 민감도 추이(체결)| |
|[국내주식]ELW시세|ELW 민감도 추이(일별)| |
|[국내주식]ELW시세|ELW 기초자산별 종목시세| |
|[국내주식]업종/기타|국내주식업종기간별시세(일/주/월/년)|⭕|
|[국내주식]업종/기타|국내휴장일조회| |
|[국내주식]업종/기타|업종분봉조회| |
|[국내주식]업종/기타|변동성완화장치(VI) 현황| |
|[국내주식]업종/기타|국내업종 현재지수| |
|[국내주식]업종/기타|국내업종 일자별지수| |
|[국내주식]업종/기타|국내업종 구분별전체시세| |
|[국내주식]업종/기타|국내주식 예상체결 전체지수| |
|[국내주식]업종/기타|국내업종 시간별지수(틱)| |
|[국내주식]업종/기타|국내업종 시간별지수(분)| |
|[국내주식]업종/기타|국내주식 예상체결지수 추이| |
|[국내주식]업종/기타|금리 종합(국내채권/금리)| |
|[국내주식]업종/기타|종합 시황/공시(제목)| |
|[국내주식]종목정보|상품기본조회| |
|[국내주식]종목정보|주식기본조회| |
|[국내주식]종목정보|국내주식 대차대조표| |
|[국내주식]종목정보|국내주식 손익계산서| |
|[국내주식]종목정보|국내주식 재무비율| |
|[국내주식]종목정보|국내주식 수익성비율| |
|[국내주식]종목정보|국내주식 기타주요비율| |
|[국내주식]종목정보|국내주식 안정성비율| |
|[국내주식]종목정보|국내주식 성장성비율| |
|[국내주식]종목정보|국내주식 당사 신용가능종목| |
|[국내주식]종목정보|예탁원정보(배당일정)| |
|[국내주식]종목정보|예탁원정보(주식매수청구일정)| |
|[국내주식]종목정보|예탁원정보(합병/분할일정)| |
|[국내주식]종목정보|예탁원정보(액면교체일정)| |
|[국내주식]종목정보|예탁원정보(자본감소일정)| |
|[국내주식]종목정보|예탁원정보(상장정보일정)| |
|[국내주식]종목정보|예탁원정보(공모주청약일정)| |
|[국내주식]종목정보|예탁원정보(실권주일정)| |
|[국내주식]종목정보|예탁원정보(의무예치일정)| |
|[국내주식]종목정보|예탁원정보(유상증자일정)| |
|[국내주식]종목정보|예탁원정보(무상증자일정)| |
|[국내주식]종목정보|예탁원정보(주주총회일정)| |
|[국내주식]종목정보|국내주식 종목추정실적| |
|[국내주식]종목정보|당사 대주가능 종목| |
|[국내주식]시세분석|국내기관_외국인 매매종목가집계| |
|[국내주식]시세분석|종목조건검색 목록조회| |
|[국내주식]시세분석|종목조건검색조회| |
|[국내주식]시세분석|종목별 프로그램매매추이(체결)| |
|[국내주식]시세분석|종목별 외인기관 추정가집계| |
|[국내주식]시세분석|종목별일별매수매도체결량| |
|[국내주식]시세분석|시장별 투자자매매동향(시세)| |
|[국내주식]시세분석|국내주식 신용잔고 일별추이| |
|[국내주식]시세분석|국내주식 예상체결가 추이| |
|[국내주식]시세분석|국내주식 공매도 일별추이| |
|[국내주식]시세분석|프로그램매매 종합현황(일별)| |
|[국내주식]시세분석|국내주식 시간외예상체결등락률| |
|[국내주식]시세분석|프로그램매매 종합현황(시간)| |
|[국내주식]시세분석|외국계 매매종목 가집계| |
|[국내주식]시세분석|종목별 외국계 순매수추이| |
|[국내주식]시세분석|국내주식 체결금액별 매매비중| |
|[국내주식]시세분석|국내 증시자금 종합| |
|[국내주식]순위분석|거래량순위| |
|[국내주식]순위분석|국내주식 등락률 순위| |
|[국내주식]순위분석|국내주식 호가잔량 순위| |
|[국내주식]순위분석|국내주식 수익자산지표 순위| |
|[국내주식]순위분석|국내주식 시가총액 상위| |
|[국내주식]순위분석|국내주식 재무비율 순위| |
|[국내주식]순위분석|국내주식 시간외잔량 순위| |
|[국내주식]순위분석|국내주식 우선주/괴리율 상위| |
|[국내주식]순위분석|국내주식 이격도 순위| |
|[국내주식]순위분석|국내주식 시장가치 순위| |
|[국내주식]순위분석|국내주식 체결강도 상위| |
|[국내주식]순위분석|국내주식 관심종목등록 상위| |
|[국내주식]순위분석|국내주식 예상체결 상승/하락상위| |
|[국내주식]순위분석|국내주식 당사매매종목 상위| |
|[국내주식]순위분석|국내주식 신고/신저근접종목 상위| |
|[국내주식]순위분석|국내주식 대량체결건수 상위| |
|[국내주식]순위분석|국내주식 공매도 상위종목| |
|[국내주식]순위분석|국내주식 신용잔고 상위| |
|[국내주식]순위분석|국내주식 배당률 상위| |
|[국내주식]순위분석|국내주식 시간외등락율순위| |
|[국내주식]순위분석|국내주식 시간외거래량순위| |
|[국내주식]실시간시세|국내주식 실시간체결가|⭕|
|[국내주식]실시간시세|국내주식 실시간호가|⭕|
|[국내주식]실시간시세|국내주식 실시간체결통보|⭕|
|[국내주식]실시간시세|국내지수 실시간체결|⭕|
|[국내주식]실시간시세|국내지수 실시간예상체결|⭕|
|[국내주식]실시간시세|국내지수 실시간프로그램매매|⭕|
|[국내주식]실시간시세|국내주식 실시간회원사|⭕|
|[국내주식]실시간시세|국내주식 실시간프로그램매매|⭕|
|[국내주식]실시간시세|국내주식 장운영정보|⭕|
|[국내주식]실시간시세|국내주식 실시간예상체결|⭕|
|[국내주식]실시간시세|ELW 실시간체결가|⭕|
|[국내주식]실시간시세|ELW 실시간호가|⭕|
|[국내주식]실시간시세|국내주식 시간외 실시간체결가|⭕|
|[국내주식]실시간시세|국내주식 시간외 실시간예상체결|⭕|
|[국내주식]실시간시세|국내주식 시간외 실시간호가|⭕|
|[국내선물옵션]주문/계좌|선물옵션 주문|⭕|
|[국내선물옵션]주문/계좌|선물옵션 정정취소주문|⭕|
|[국내선물옵션]주문/계좌|선물옵션 주문체결내역조회|⭕|
|[국내선물옵션]주문/계좌|선물옵션 잔고현황|⭕|
|[국내선물옵션]주문/계좌|선물옵션 주문가능|⭕|
|[국내선물옵션]주문/계좌|(야간)선물옵션 주문체결내역조회| |
|[국내선물옵션]주문/계좌|(야간)선물옵션 잔고현황| |
|[국내선물옵션]주문/계좌|(야간)선물옵션 주문가능| |
|[국내선물옵션]주문/계좌|선물옵션 잔고정산손익내역| |
|[국내선물옵션]주문/계좌|선물옵션 총자산현황| |
|[국내선물옵션]주문/계좌|선물옵션 잔고평가손익내역| |
|[국내선물옵션]주문/계좌|선물옵션 기준일체결내역| |
|[국내선물옵션]주문/계좌|선물옵션기간약정수수료일별| |
|[국내선물옵션]기본시세|선물옵션 시세|⭕|
|[국내선물옵션]기본시세|선물옵션 시세호가|⭕|
|[국내선물옵션]기본시세|선물옵션기간별시세(일/주/월/년)|⭕|
|[국내선물옵션]기본시세|선물옵션 분봉조회| |
|[국내선물옵션]기본시세|선물옵션 일중예상체결추이| |
|[국내선물옵션]기본시세|국내선물 기초자산 시세|⭕|
|[국내선물옵션]기본시세|국내옵션전광판_옵션월물리스트| |
|[국내선물옵션]기본시세|국내옵션전광판_선물| |
|[국내선물옵션]실시간시세|지수선물 실시간체결가| |
|[국내선물옵션]실시간시세|지수선물 실시간호가| |
|[국내선물옵션]실시간시세|선물옵션 실시간체결 통보| |
|[국내선물옵션]실시간시세|지수옵션 실시간체결가| |
|[국내선물옵션]실시간시세|지수옵션 실시간호가| |
|[국내선물옵션]실시간시세|상품선물 실시간체결가| |
|[국내선물옵션]실시간시세|상품선물 실시간호가| |
|[국내선물옵션]실시간시세|주식선물 실시간체결가| |
|[국내선물옵션]실시간시세|주식선물 실시간호가| |
|[국내선물옵션]실시간시세|주식옵션 실시간체결가| |
|[국내선물옵션]실시간시세|주식옵션 실시간호가| |
|[해외주식]주문/계좌|해외주식 주문|⭕|
|[해외주식]주문/계좌|해외주식 정정취소주문|⭕|
|[해외주식]주문/계좌|해외주식 예약주문접수|⭕|
|[해외주식]주문/계좌|해외주식 예약주문접수취소|⭕|
|[해외주식]주문/계좌|해외주식 미체결내역|⭕|
|[해외주식]주문/계좌|해외주식 잔고|⭕|
|[해외주식]주문/계좌|해외주식 주문체결내역|⭕|
|[해외주식]주문/계좌|해외주식 체결기준현재잔고|⭕|
|[해외주식]주문/계좌|해외주식 예약주문조회| |
|[해외주식]주문/계좌|해외주식 매수가능금액조회| |
|[해외주식]주문/계좌|해외주식 미국주간주문| |
|[해외주식]주문/계좌|해외주식 미국주간정정취소| |
|[해외주식]주문/계좌|해외주식 기간손익| |
|[해외주식]기본시세|해외주식 현재체결가|⭕|
|[해외주식]기본시세|해외주식 기간별시세|⭕|
|[해외주식]기본시세|해외주식 종목/지수/환율기간별시세(일/주/월/년)|⭕|
|[해외주식]기본시세|해외주식 조건검색|⭕|
|[해외주식]기본시세|해외결제일자조회| |
|[해외주식]기본시세|해외주식 현재가상세| |
|[해외주식]기본시세|해외주식분봉조회| |
|[해외주식]기본시세|해외지수분봉조회| |
|[해외주식]기본시세|해외주식 상품기본정보| |
|[해외주식]기본시세|해외주식 현재가 10호가| |
|[해외주식]시세분석|해외주식 기간별권리조회| |
|[해외주식]시세분석|해외뉴스종합(제목)| |
|[해외주식]실시간시세|해외주식 실시간지연체결가| |
|[해외주식]실시간시세|해외주식 실시간지연호가(아시아)| |
|[해외주식]실시간시세|해외주식 실시간체결통보| |
|[해외주식]실시간시세|해외주식 실시간호가(미국)| |
|[해외선물옵션]주문/계좌|해외선물옵션 주문| |
|[해외선물옵션]주문/계좌|해외선물옵션 정정취소주문| |
|[해외선물옵션]주문/계좌|해외선물옵션 당일주문내역조회| |
|[해외선물옵션]주문/계좌|해외선물옵션 미결제내역조회(잔고)| |
|[해외선물옵션]주문/계좌|해외선물옵션 주문가능조회| |
|[해외선물옵션]주문/계좌|해외선물옵션 기간계좌손익 일별| |
|[해외선물옵션]주문/계좌|해외선물옵션 일별 체결내역| |
|[해외선물옵션]주문/계좌|해외선물옵션 예수금현황| |
|[해외선물옵션]주문/계좌|해외선물옵션 일별 주문내역| |
|[해외선물옵션]주문/계좌|해외선물옵션 기간계좌거래내역| |
|[해외선물옵션]기본시세|해외선물종목상세|⭕|
|[해외선물옵션]기본시세|해외선물종목현재가|⭕|
|[해외선물옵션]기본시세|해외선물 분봉조회| |
|[해외선물옵션]기본시세|해외선물옵션 체결추이(주간)| |
|[해외선물옵션]기본시세|해외선물옵션 체결추이(일간)| |
|[해외선물옵션]기본시세|해외선물옵션 체결추이(틱)| |
|[해외선물옵션]기본시세|해외선물옵션 체결추이(월간)| |
|[해외선물옵션]기본시세|해외선물 호가| |
|[해외선물옵션]실시간시세|해외선물옵션 실시간체결가| |
|[해외선물옵션]실시간시세|해외선물옵션 실시간호가| |
|[해외선물옵션]실시간시세|해외선물옵션 실시간주문내역통보| |
|[해외선물옵션]실시간시세|해외선물옵션 실시간체결내역통보| |
  
## 4. API 예제 목록

|구분|예제명|지원언어|
|--|--|--|
|rest|kis_api.py|python|
|rest|reauth.py|python|
|websocket|ops_ws_sample.jar|java|
|websocket|ops_ws_sample.html|js|
|websocket|ops_ws_sample.py|python|
|websocket|ws_domestic+overseas_stock.py|python|
|websocket|ws_domestic_stock.py|python|
|websocket|ws_overseas_stock.py|python|
|websocket|ws_real_multiple_stocks.py|python|
|websocket|ws_realstkprice.py|python|
|websocket|ws_realstkquote.py|python|

## 5. Wikidocs(참고 교안)
|구분|도서명|지원언어|링크|
|--|--|--|--|
|rest|파이썬으로 배우는 오픈API 트레이딩 초급 예제|python|https://wikidocs.net/book/7559|
|websocket|파이썬으로 배우는 한국투자증권 Websocket 사용 예제|python|https://wikidocs.net/book/7847|


![Footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&height=200&section=footer)
