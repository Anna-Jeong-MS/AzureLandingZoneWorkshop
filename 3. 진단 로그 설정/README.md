# 3. 진단 로그 설정

## Log Analytics 작업 영역 생성

1. **Log Analytics 작업 영역 화면**으로 이동합니다.
2. 왼쪽 상단 `만들기` 버튼을 클릭합니다.
3. 다음과 같이 설정 후 `리뷰 + 만들기` 버튼을 클릭하여 리소스를 생성합니다.
    - 구독 : 할당 받은 구독 선택
    - 리소스 그룹 : 생성한 본인 리소스 그룹 선택
    - 이름 : `LogWorkspace`
    - 영역 : Korea Central

## 방화벽 로그 설정

1. **방화벽 화면**으로 이동 후 생성한 방화벽을 클릭합니다.
2. 왼쪽 메뉴에서 `진단 설정`을 선택합니다.
3. `+ 진단 설정 추가`를 클릭합니다.
4. 아래와 같이 설정 후 `저장` 버튼을 클릭합니다.
    - 진단 설정 이름 : `FirewallLogs`
    - 범주 그룹 : AllLogs
    - 메트릭 : AllMetrics
    - 대상 세부 정보 : Log Analytics 작업 영역에 보내기
        - 구독 : 생성한 구독 선택
        - Log Analytics 작업 영역 : LogWorkspace ( koreacentral)
        - 대상 테이블 : Azure 진단

## WAF 로그 설정

1. **애플리케이션 게이트웨이 화면**으로 이동 후 생성한 애플리케이션 게이트웨이를 클릭합니다.
2. 왼쪽 메뉴에서 `진단 설정`을 선택합니다.
3. `+ 진단 설정 추가`를 클릭합니다.
4. 아래와 같이 설정 후 `저장` 버튼을 클릭합니다.
    - 진단 설정 이름 : `WAFLogs`
    - 범주 그룹 : AllLogs
    - 메트릭 : AllMetrics
    - 대상 세부 정보 : Log Analytics 작업 영역에 보내기
        - 구독 : 생성한 구독 선택
        - Log Analytics 작업 영역 : LogWorkspace ( koreacentral)
        - 대상 테이블 : Azure 진단