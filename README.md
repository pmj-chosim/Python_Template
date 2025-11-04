# Python_Template


### 0. 사전 준비  

VSC와 Python 환경이 로컬 컴퓨터에 설치 되어 있는 경우, 아래 명령어를 통해 예제 폴더를 다운받습니다. 
```
git clone https://github.com/pmj-chosim/Python_Template.git
```
만약, 환경이 없다면 아래 단계를 차례대로 수행해 주세요.  

(https://github.com/pmj-chosim/Python_Template)[https://github.com/pmj-chosim/Python_Template]에 접속합니다.  
이후, fork 버튼을 누르고 create fork 버튼을 클릭합니다.  
<img width="1507" height="442" alt="image" src="https://github.com/user-attachments/assets/ad15647d-bb09-4b78-8fb6-a62adf85a8bc" />  
<img width="967" height="745" alt="image" src="https://github.com/user-attachments/assets/58edeacc-8347-4db8-b45e-0d4eb9518b6a" />  

Code > Codespaces > Create codespaces on main을 선택합니다.  
<img width="1202" height="696" alt="image" src="https://github.com/user-attachments/assets/28835052-2bed-495a-a556-5bfeb0010773" />  

환경이 셋팅될 때까지 기다립니다.  
<img width="1882" height="833" alt="image" src="https://github.com/user-attachments/assets/5b101e8f-484f-4506-b1ee-54ceba62655f" />  
  

---

### 1. 요금제 확인
먼저, 실습하기 앞서 현재 사용하고 있는 요금제를 확인해보겠습니다.  

우측 상단에 있는 프로필 사진을 클릭합니다.   
<img width="798" height="742" alt="image" src="https://github.com/user-attachments/assets/8d2498d7-a58f-46f6-a40a-73de821f505e" />  <br>  
  
`Settings`를 클릭합니다.  <br>  
<img width="981" height="617" alt="image" src="https://github.com/user-attachments/assets/6a4777d1-cbdc-4b62-b398-d22e3a4731ca" />  <br>   
`Access`의 `Licensing`을 선택합니다.   

`Current GitHub base plan` 섹션에서 현재 계정의 플랜을 확인할 수 있습니다.  
<br>

### 2. GitHub Copilot 설치하기  
GitHub Copilot을 설치해 보겠습니다.  

아래 사진과 같이 좌측의 확장 버튼을 누른 후, `github copilot`을 검색하여 `설치`합니다.  
<img width="1234" height="512" alt="image" src="https://github.com/user-attachments/assets/77b2e000-687a-4380-96de-701d07a827c1" />  


설치가 완료되면, 우측에 다음과 같은 채팅창이 나타납니다.  
<img width="1738" height="840" alt="image" src="https://github.com/user-attachments/assets/02de0447-2250-4b19-b209-94ad9c6403fd" />  


### 3. GitHub Copilot 기능 살펴 보기  
- 코드 완성 기능
- 채팅

이 두 가지 기능을 각각 실습을 통해 살펴 봅니다.  
실습 전, 실습을 할 수 있도록 새로운 프로젝트를 먼저 열어 봅니다.  

#### (1) 코드 완성 기능  
코드 완성 기능은 사용자가 코드를 작업하는 공간에서 코드를 제안 받는 것입니다. 주석을 작성하거나 자동 작성을 통해 코드를 완성할 수 있습니다.  

- 주석을 통해 원하는 기능을 자동으로 제안 받을 수 있습니다.  
새로 생성한 Python 프로젝트에 main.py와 같은 Python 파일을 만듭니다. 해당 파일에 아래와 같이 주석을 작성합니다.
<img width="436" height="407" alt="image" src="https://github.com/user-attachments/assets/d0952cd1-52d1-4096-8b32-352f69d72b0c" />
```python
# 출력 완료 메시지를 보여줍니다.
```
<img width="1073" height="226" alt="image" src="https://github.com/user-attachments/assets/693e4826-42db-47fc-9c40-b27a7fc89fc3" />  

주석을 작성한 후 `Enter`를 눌러 다음 줄로 이동합니다. Copilot이 `print("출력 완료!")`와 같이 코드를 제안할 것입니다. 키보드의 `Tab` 버튼을 눌러 제안을 수락합니다.  
<img width="643" height="181" alt="image" src="https://github.com/user-attachments/assets/d0390e82-0e0a-4ab4-be6f-96340528d08e" />  


- 코드를 작성하는 와중에도 코드를 제안 받을 수 있습니다.
```python
sum_value_one_to_ten = 0
```
위 코드를 앞서 실습했던 내용 뒤에 붙여 넣어 주세요. 코드를 붙여 넣고 나서, 키보드의 Enter 버튼을 누릅니다.  
<img width="675" height="200" alt="image" src="https://github.com/user-attachments/assets/42d7e67a-9f2e-4445-b8a7-650b52f6c47c" />    
  
`Enter` 버튼을 누르면 Copilot이 1부터 10까지 더하는 for 루프와 같은 다음 코드를 제안할 수 있습니다. `Tab` 버튼을 눌러 Copilot의 제안을 수락합니다.  
<img width="725" height="272" alt="image" src="https://github.com/user-attachments/assets/cb73c308-f862-415d-8d04-74c41cc09058" />  
<img width="670" height="263" alt="image" src="https://github.com/user-attachments/assets/89781c95-0db5-4797-b6e8-3965fc61deea" />  

<br>  

#### (2) 채팅 기능
채팅은 다음 4가지 방법을 통해 사용할 수 있습니다.  

- 채팅 뷰
- 인라인 채팅
- 스마트 액션
- 퀵 채팅

위 방법들을 순차적으로 실습을 통해 살펴 보겠습니다.  

- 채팅 뷰
IntelliJ(PyCharm)에서 우측의 GitHub Copilot 버튼을 눌러 채팅을 엽니다. 채팅 뷰에서 모드를 **Ask**, 모델은 GPT 4.1로 선택합니다.  

```bash
계산기 기능을 가진 python 어플리케이션을 만들어 주세요
```
<img width="1447" height="368" alt="image" src="https://github.com/user-attachments/assets/03c535c1-53d7-44bf-a073-ad8a69952f95" />    
<img width="486" height="783" alt="image" src="https://github.com/user-attachments/assets/df670aa7-1b88-4481-a3df-bbab2d21a9e7" />  
라고 채팅창에 입력합니다. 채팅 창에 코드를 제시하며 설명을 해줄 것입니다.  
  
`Agent` 모드로 바꾼 다음 동일한 질문을 해보겠습니다. `Agent` 모드로 바꾼 후
 

  

 


 







