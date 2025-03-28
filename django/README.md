# Django 프로젝트 가이드

이 프로젝트는 Django 웹 프레임워크를 사용한 웹 애플리케이션입니다.

## 환경 설정

### Python 가상환경 설정
```bash
# 가상환경 생성
python -m venv venv

# 가상환경 활성화
# Windows
venv\Scripts\activate
# Linux/Mac
source venv/bin/activate
```

### 필요한 패키지 설치
```bash
pip install django
```

## 프로젝트 시작하기

### Django 프로젝트 생성
```bash
django-admin startproject config .
```

### 앱 생성
```bash
python manage.py startapp main
```

### 데이터베이스 마이그레이션
```bash
python manage.py makemigrations
python manage.py migrate
```

### 개발 서버 실행
```bash
python manage.py runserver
```

서버가 실행되면 http://127.0.0.1:8000 에서 웹사이트를 확인할 수 있습니다.

## 프로젝트 구조
```
django/
├── config/          # 프로젝트 설정 디렉토리
├── main/           # 메인 앱 디렉토리
├── manage.py       # Django 관리 스크립트
├── venv/           # 가상환경 디렉토리
└── README.md       # 이 파일
```

## 유용한 Django 명령어
- `python manage.py createsuperuser`: 관리자 계정 생성
- `python manage.py shell`: Django 쉘 실행
- `python manage.py collectstatic`: 정적 파일 수집
- `python manage.py test`: 테스트 실행

## 참고 자료
- [Django 공식 문서](https://docs.djangoproject.com/)
- [Django 튜토리얼](https://docs.djangoproject.com/ko/4.2/intro/tutorial01/) 