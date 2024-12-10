# Windows에서 Docker 설치

이 가이드는 Windows에서 Docker를 설치하고 GPU를 사용할 수 있는 Docker 환경을 설정하는 방법을 설명합니다.

> **주의:** 이 가이드는 Windows 시스템에 WSL이 이미 설치되어 있다는 전제 하에 작성되었습니다.
>
> WSL이 설치되어 있지 않다면, [WSL 설치 가이드 1](https://github.com/sw-dreamer/wsl-install.git) 나 [WSL 설치 가이드 2](https://docs.microsoft.com/en-us/windows/wsl/install)를 참조하여 먼저 WSL을 설치하십시오.

## 1. Docker Desktop 다운로드

Docker를 Windows에 설치하려면 다음 단계를 따릅니다:

1. 아래 링크를 클릭하여 Docker Desktop을 다운로드합니다:
   - [Docker Desktop for Windows](https://www.docker.com/products/docker-desktop/)

2. 웹 페이지에서 **Download for Windows** 버튼을 클릭하여 설치 파일을 다운로드합니다.

## 2. Docker Desktop 설치

1. 다운로드한 설치 파일을 실행하여 Docker Desktop을 설치합니다.
2. 설치가 완료되면 프로그램을 실행합니다.
3. Docker Desktop을 실행하면 진행 과정 중에 컴퓨터가 자동으로 로그아웃됩니다.

> **참고:** Docker Desktop은 WSL 2를 기반으로 작동하므로, WSL이 정상적으로 설치되어 있어야 합니다.

## 3. Docker Desktop에서 WSL 2 통합 활성화

Docker Desktop을 설치한 후에는 WSL 2 통합을 활성화해야 합니다

1. Docker Desktop을 열고, 오른쪽 상단의 설정(gear 아이콘) 을 클릭합니다.
   
2. General 탭에서 WSL 2 기반 엔진 사용 옵션이 활성화되어 있는지 확인합니다.
   
3. Resources 탭으로 이동한 후 WSL Integration을 활성화합니다.
   
   이 옵션에서 Docker와 통합할 WSL 배포판을 선택할 수 있습니다.
   
   현재 사용 중인 배포판이 선택되어 있는지 확인하세요.

## 4. Docker 설치 확인

Window키 + S 를 눌러서 ubuntu를 검색 후 로그인을 합니다. 그리고 아래 명령어로 docker가 정상적으로 설치 되어있는지 확인합니다.

   ```bash
   docker --version
   ```

이 명령어를 실행한 후, **Docker version 27.3.1, build ce12230**식으로 출력이 되면 정상적으로 설치 된 것입니다.

## 5. 결론

이 가이드를 통해 Docker Desktop을 설치하고 사용할 수 있는 Docker 환경을 설정했습니다.
