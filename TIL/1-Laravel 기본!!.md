# Laravel 기본!!

## 1. Laravel 프로젝트 시작 전
	Laravel을 다운받는 방법은 여러가지지만
	필자는 Composer를 활용한 방법을 작성한다.
	
	우선!! Composer를 다운로드 받기 위해선 php가 필요하다.
	Local환경이든 가상환경이든 접근가능한 형태로 php를 설치하도록 한다.
	composer 또한 인터넷에 검색하면 바로 다운로드 받을 수 있다.
	필자는 Windows + nginx + php + mariadb를 받을 수 있는 WNMP를 추천한다.
	따라서 WNMP 다운로드 -> Composer 다운로드 순으로 진행하면 되겠다.
	
	Composer를 다운로드 받았다면 composer 명령어가 활성된다.
	composer -v (버전을 먼저 확인해보고)
	composer create-project laravel/laravel '프로젝트명'
	
	필자는 라라벨 7점대의 버전을 활용한다.
	라라벨은 패치에 따라서 backend와 frontend를 분리해서 관리한다.
	composer는 백엔드 의존성관리이고 npm은 프론트 의존성을 관리한다.
	따라서!! npm이 필요하다.
	npm은 node.js를 받으면 자동으로 딸려온다.
	다운로드 받으면 npm 명령어가 활성화된다.
	
	미리 생성한 프로젝트 디렉토리에서 실행하도록한다.
	npm install   (npm에서 제공하는 프론트엔드 스캐폴딩을 활용하기위함이다.)
	npm run --dev (프로젝트의 sass등의 프론트관련 설정을 실행하여 public에 위치시킨다.)
	
	composer require laravel/ui --dev (laravel의 프로젝트에 ui를 추가한다.)
	php artisan ui vue [--auth] (프로젝트에서 vue의존성을 추가한다. --auth를 입력하면 계정관리 페이지생성)