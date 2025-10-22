# 🚀 Google Colab 완전 가이드 (Complete Guide to Google Colab)

> 💡 이 문서는 Google Colab을 처음 사용하는 사람부터, 효율적으로 활용하고 싶은 개발자까지 모두를 위한 종합 가이드입니다.  
> ✅ 예제 코드, 환경 설정, GPU 활용법, GitHub 연동까지 단계별로 정리했습니다.

---

## 📚 목차

| 구분 | 내용 | 바로가기 |
|------|------|-----------|
| 1️⃣ | Colab 소개 및 시작하기 | [Colab 소개](#-colab-소개-및-시작하기) |
| 2️⃣ | 환경 설정 및 기본 기능 | [환경 설정](#-환경-설정-및-기본-기능) |
| 3️⃣ | 파일 입출력 & Google Drive 연동 | [파일 I/O](#-파일-입출력--google-drive-연동) |
| 4️⃣ | GPU / TPU 설정 | [GPU/TPU 설정](#-gpu--tpu-설정) |
| 5️⃣ | GitHub와 연동 | [GitHub 연동](#-github와-연동) |
| 6️⃣ | 유용한 팁 & 단축키 | [유용한 팁](#-유용한-팁--단축키) |
| 7️⃣ | 자주 발생하는 오류 해결 | [오류 해결](#-자주-발생하는-오류-해결) |

---

## 🧠 Colab 소개 및 시작하기

| 항목 | 내용 |
|------|------|
| **Colab이란?** | Google이 제공하는 클라우드 기반 Python 실행 환경 (Jupyter Notebook 기반). |
| **특징** | 무료 GPU/TPU 제공, 구글 계정만 있으면 바로 사용 가능. |
| **접속 경로** | 👉 [https://colab.research.google.com](https://colab.research.google.com) |
| **필요한 것** | Google 계정, 인터넷 브라우저 (Chrome 권장). |

**🔹 새 노트북 만들기**
1. [Colab 사이트](https://colab.research.google.com) 접속  
2. `파일(File)` → `새 노트북(New notebook)` 클릭  
3. Python 코드 입력 후 `Shift + Enter`로 실행

---

## ⚙️ 환경 설정 및 기본 기능

| 기능 | 설명 | 예시 코드 |
|------|------|-----------|
| **Python 버전 확인** | 현재 런타임의 Python 버전 확인 | `!python --version` |
| **패키지 설치** | pip 명령어로 라이브러리 설치 | `!pip install numpy pandas` |
| **시스템 정보** | CPU/GPU 메모리 확인 | `!nvidia-smi`, `!cat /proc/meminfo` |

**🔸 노트북 환경 확인 코드 예시**
```python
import platform, psutil
print("Python:", platform.python_version())
print("CPU:", psutil.cpu_count(), "cores")
