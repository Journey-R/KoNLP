# KoNLPy 패키지 설치



### KoNLPy : 한글 자연어 처리 패키지

#### * 한글 형태소 분석기 종류

- Hannanum
- Kkma
- Komoran
- Okt



### 설치 방법 (공홈)

https://konlpy-ko.readthedocs.io/ko/v0.5.1/install/#id2

- 공홈의 Windows 설치 방법 따라 설치시 오류 발생하여 아래의 방법으로 설치 진행
  - Error : PackagesNotFoundError (오류 관련 내용은 하단에 기재)



---



### (1) KoNLPy 패키지 설치 에러 발생

- **PackagesNotFoundError** 오류 발생하여 아래의 방법으로 해결
  - 참고 : Error : PackageNotFoundError



### 설치 순서 (PyCharm Terminal 통한 패키지 설치)

1. **JDK 설치** (Java 1.7 이상인 버전 미설치시)

   - https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html

   

2. **환경 변수 설정**

   1. [시스템 속성] - [고급] - [환경변수] - [시스템 변수] - [새로 만들기]
   2. ![image](https://user-images.githubusercontent.com/71396432/108505268-75e0f680-72fa-11eb-9643-3347f1cbff5d.png)

   

3. **JPype1 설치 (버전 : 0.5.7 이상)** 

   - https://www.lfd.uci.edu/~gohlke/pythonlibs/#jpype
   - 설치할 파일 선택
     - cp[**파이썬 버전**] : 3.8 버전 -> cp38
     - win[**32 or 64**] : 32bit -> win32, 64bit -> amd64
     - 예 : python 3.8 버전, OS 64bit -> **JPype1-1.2.0-cp38-cp38-win_amd64.whl**

   - python version

     - 패키지를 사용할 프로젝트에서 사용하는 파이썬 버전 확인

       (Anaconda Prompt와 프로젝트의 python  버전이 상이할 경우 해당 프로젝트의 버전을 따름)

       1. PyCharm Open

       2. [File] - [Settings] - [Project : Name] - [Project Interpreter] - [Package] - [Python]

          ![image](https://user-images.githubusercontent.com/71396432/108506697-90b46a80-72fc-11eb-8cce-c627d941b616.png)

4. **현재 작업 중이 프로젝트 디렉토리에 저장**

   

5. **PyCharm Terminal**

   

6. **JPype 설치**

   ```
   python -m pip install JPype1-1.2.0-cp38-cp38-win_amd64.whl
   ```

   ![image](https://user-images.githubusercontent.com/71396432/108507454-afffc780-72fd-11eb-94af-8c244a6c00c7.png)

   

7. **KoNLPy 설치**

   ```
   python -m pip install konlpy
   ```



