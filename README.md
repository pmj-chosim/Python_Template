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
라고 채팅창에 입력합니다. 채팅 창에 코드를 제시해 줄 것입니다.      
<img width="507" height="777" alt="image" src="https://github.com/user-attachments/assets/ccc73667-d245-4e8d-99e1-975ceb392c4f" />  

  
`Agent` 모드로 바꾼 다음 동일한 질문을 해보겠습니다. `Agent` 모드로 바꾼 후  

```bash
계산기 기능을 가진 python 어플리케이션을 만들어 주세요
```

<img width="1478" height="784" alt="image" src="https://github.com/user-attachments/assets/8a229d84-836b-4b6d-b70d-45d9a96bba89" />   
<img width="1478" height="784" alt="image" src="https://github.com/user-attachments/assets/69249064-c84d-43dd-ae17-830bc6850c14" />  


다시 동일한 질문을 같이 해보았습니다.

`Ask` 모드는 채팅창에서 코드나 답을 제시했었습니다. 이와 달리 `Agent` 모드에선 "계산기 앱 만들어 줘"라고 하면 main.py 파일에 계산기 코드를 넣어 줍니다. 그냥 구경하는 게 아니라 직접 일을 해주는 `Agent`처럼 동작합니다.

지금과 같이 `main.py` 하나만 있는 간단한 프로젝트는 물론이고, 파일이 여러 개 섞여서 머리 아픈 복잡한 프로젝트도 문제없이 수정해줍니다. `Agent` 모드는 여러 내용들을 쫙 훑어보고 어디를 어떻게 고쳐야 할지 스스로 판단해서 여러 파일을 넘나들며 수정해주기 때문입니다.  

`Edit` 모드도 사용해보겠습니다. 채팅에서 `Edit`을 선택해 모드를 변경하려고 하면, 변경 사항을 저장할지 묻는 팝업이 뜰 수 있습니다. `Discard` 버튼을 누릅니다.    
<img width="502" height="770" alt="image" src="https://github.com/user-attachments/assets/552287ac-4046-403a-87f2-007e861b261a" />  

<img width="1448" height="762" alt="image" src="https://github.com/user-attachments/assets/ff6bfb2a-ece2-438e-8df0-04fab4ce3f60" />


클립 버튼을 누른 후, `main.py` 파일을 선택합니다. `main.py` 파일을 더블 클릭하면 파일을 추가할 수 있습니다. 
<img width="463" height="158" alt="image" src="https://github.com/user-attachments/assets/7768b65c-c990-4a48-a2a5-0efad4d9e2a4" />  
<img width="1063" height="821" alt="image" src="https://github.com/user-attachments/assets/499d80e5-414f-4705-bbf8-89a7d6b5f469" />  


그 다음 채팅창에
```bash
계산기 기능을 확장해 주세요  
```
<img width="486" height="167" alt="image" src="https://github.com/user-attachments/assets/08dd8a03-c909-4ade-b674-5575fe4ba38c" />  
이 질문을 다시 붙여 넣고 물어 보겠습니다.  

아까 선택했던 `main.py`의 코드들을 수정하는 제안을 보여줄 것입니다. Accept All 버튼을 눌러 수정 제안을 받아 들입니다.  
<img width="1523" height="782" alt="image" src="https://github.com/user-attachments/assets/01d9651c-7866-473e-87fb-8c141d25286b" />  


`Edit`에서는 선택한 main.py 코드에서 필요한 부분만 수정했을 것입니다. 반면, `Agent`도 작업 공간의 코드를 변경했습니다. 다만, 사용자가 따로 파일을 지정하지 않아도 스스로 필요한 파일을 찾아 여러 파일을 넘나들며 수정한다는 점에서 차이가 있습니다.  

채팅 뷰의 3가지 모드에 대해서 살펴 보았습니다. `Ask` 모드는 채팅창에서 코드나 답을 제시하는 역할을 합니다. `Agent` 모드는 여러 코드들을 이해하고 코드를 직접 수정해줍니다. 더불어, 코드 작성뿐만 아니라 필요한 라이브러리 설치(예: pip install...) 등과 같은 환경 설정까지, 다양한 작업을 처리해주는 실제 대행자처럼 동작합니다. 그리고 `Edit` 모드는 사용자가 지정한 파일에 대해서 또는 `Agent` 보다는 좁은 맥락에서 코드를 수정한다는 차이점이 있었습니다.  


- 인라인 채팅  
인라인 채팅은 코드를 작성하는 도중에 바로 코드 편집기 안에서 코파일럿과 대화하는 기능입니다. 별도의 채팅 창을 열지 않고도 특정 코드 블록이나 함수 옆에서 곧바로 질문하고 답변을 받을 수 있습니다.  

예를 들어, 어떤 함수의 기능이 궁금할 때, 그 함수 위에 커서를 두고 인라인 채팅을 활성화해서 "이 함수는 무슨 역할을 해?"라고 물어볼 수 있습니다. 그러면 코파일럿이 바로 옆에 답변을 띄워주는 식으로 동작합니다.  

이 기능은 코딩 흐름을 끊지 않고 필요한 정보를 얻거나, 코드 수정에 대한 도움을 받고 싶을 때 매우 유용합니다.  

`main.py` 파일의 코드 편집기 내부에서 마우스 우클릭을 합니다. GitHub Copilot 메뉴가  뜰 것입니다. 메뉴에서 인라인 채팅 열기를 클릭합니다.  
<img width="627" height="282" alt="image" src="https://github.com/user-attachments/assets/af7cfb91-c034-44d5-8f31-c851278b2cf3" />  


그리고  
```bash
지금 코드 동작을 간략하게 설명해줘
```
라고 입력합니다.
<img width="833" height="348" alt="image" src="https://github.com/user-attachments/assets/18eb1e10-4ce4-4020-863a-92f8f410a7bb" />    
  
인라인 채팅을 사용하면 코드 작업 공간에서 편리하게 원하는 질문을 할 수 있음을 실습을 통해 알아 보았습니다.  

  
- 스마트 액션
스마트 액션은 GitHub Copilot을 통해 받고 싶은 도움을 귀찮게 채팅을 치지 않아도 쉽게 받을 수 있게 하는 방법입니다.  


코드 작업 공간에서 원하는 코드 블록을 드래그하여 선택한 후, 마우스 우클릭을 하면 GitHub Copilot 메뉴가 뜰 것입니다.  
<img width="442" height="308" alt="image" src="https://github.com/user-attachments/assets/dfb3330f-1116-475b-abf8-acffde21e430" />   
<img width="537" height="303" alt="image" src="https://github.com/user-attachments/assets/e5224558-82a0-4484-9810-fc706ed1926f" />  


메뉴를 살펴보면 Simplify This(간소화), Generate Docs(문서/주석 생성), Generate Tests(테스트 생성), Fix This(오류 수정), Explain This(설명) 등을 확인할 수 있습니다. 이 메뉴들을 선택하면 요약, 문서 생성 등의 동작들을 채팅을 치지 않고 요청할 수 있습니다. 앞서 인라인 채팅 실습에선 채팅으로 직접 설명을 하라고 요청했습니다.  
<img width="702" height="407" alt="image" src="https://github.com/user-attachments/assets/27203119-aeff-4130-87d0-f64159bdbb11" />  


하지만, 이 스마트 액션을 통해 채팅을 입력하지 않고도 요약을 요청해보겠습니다. 설명받고 싶은 코드를 드래그한 후, 마우스 우클릭 > Explain 를 선택합니다.   

해당 코드에 대한 설명을 채팅을 입력하지 않아도 얻을 수 있습니다.  
<img width="1563" height="667" alt="image" src="https://github.com/user-attachments/assets/2d441aa2-aadd-4708-9d60-4c6c3441a334" />  


- 퀵 채팅

퀵 채팅(Quick Chat)은 별도의 챗봇 창(사이드바)을 열지 않고, 편집기 화면 위에 바로 작은 부동 채팅창을 띄워 대화하는 기능입니다.  

코딩 중인 작업 흐름을 끊지 않고, 현재 화면을 벗어나지 않은 상태에서 빠르게 질문하고 싶을 때 매우 유용합니다.
<img width="1256" height="363" alt="image" src="https://github.com/user-attachments/assets/946b3cc5-20db-4bd2-adff-324db89285e2" />

상단의 채팅 옵션에서 **빠른 채팅 열기**를 클릭하면 퀵 채팅을 열 수 있습니다. (VS Code 기본 단축키: Cmd+Shift+I 또는 Ctrl+Shift+I)  

<img width="920" height="298" alt="image" src="https://github.com/user-attachments/assets/44600c38-5d0d-4619-abde-530db34e66b3" />  

이 기능은 다음과 같은 특징이 있습니다.

- 작업 흐름 유지: 전체 사이드바를 열어 화면을 가리지 않기 때문에, 현재 작업 중인 코드를 계속 보면서 질문하고 답변을 확인할 수 있습니다.  
- 빠른 접근성: 단축키나 메뉴 클릭 한 번으로 즉시 채팅창을 불러올 수 있어 신속합니다.  
- 간결한 사용성: 채팅 뷰(사이드바)의 Ask 모드와 유사하게 동작하지만, 인터페이스가 더 간결하고 가볍습니다. 일반적인 질문이나 간단한 코드 스니펫에 대한 질문을 하기에 적합합니다.  







 


  

 


 







