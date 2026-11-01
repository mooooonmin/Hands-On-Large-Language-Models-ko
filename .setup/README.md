# 설치 안내

이 문서에서는 책에 나오는 코드를 실행하는 여러 방법을 소개합니다. 권장하는 방법은 두 가지로, 하나는 로컬용이고 다른 하나는 클라우드용입니다:

* **로컬**: [Conda](../.setup/conda) 환경 사용
* **클라우드**: [Google Colab 노트북](../README.md#목차) 사용

## 빠른 시작

로컬에 이미 파이썬(3.10.*) 환경과 [Microsoft Visual C++ 14.0](https://visualstudio.microsoft.com/visual-cpp-build-tools/) 이상이 설치되어 있다면, 이 저장소의 루트에서 다음 명령으로 전체 환경을 설치할 수 있습니다:

```bash
pip install -r requirements.txt
```

> [!WARNING]
> `error: Microsoft Visual C++ 14.0 or greater is required.` 오류가 발생하면 C++를 설치해야 합니다.
> 환경을 설치하기 전에 [여기](../.setup/conda/common_issues.md)의 설치 가이드를 따라 주세요.

conda가 설치되어 있다면(이 경우 C++를 따로 설치할 필요가 **없습니다**), 이 저장소의 루트에서 다음 명령으로 전체 환경을 설치할 수도 있습니다:

```bash
conda env create -f environment.yml
```

> [!TIP]
> 대부분의 예제는 GPU가 필요하므로, 환경을 준비한 뒤 [여기](https://pytorch.org/)의 안내에 따라 GPU 버전 PyTorch를 설치하는 것을 권장합니다.

환경 설정에 대한 전체 튜토리얼은 [conda 예제](../.setup/conda)를 참고하세요.
