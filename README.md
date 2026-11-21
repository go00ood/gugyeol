# 날개셋 구결자 입력

![구결자 입력](https://raw.githubusercontent.com/go00ood/gugyeol/main/구결자%20입력.gif)

- `리`, `뎌` 등의 독음이나 `ㄱ`, `ㄷ` 등 초성을 입력 -> `shift+한자`를 눌러 구결자 변환
- 날개셋 버전 10.7 (2024년 4월 29일)로 진행. 버전이 다르거나 안되는 경우 아래 참조.

- [해결방법](#입력기-종합설정-변경)


## 설정 방법
## 구결자 파일 다운로드
- [날개셋 구결자 파일](https://github.com/go00ood/gugyeol/blob/main/nalgaeset%20gugyeol%20261121.txt)에 접속
- 파일 오른쪽 상단의 **Download raw file** 아이콘(<escape>↓</escape>)을 클릭
  - 다운로드 아이콘이 보이지 않으면 **Raw** 버튼 옆 메뉴(`...`)에서 다운로드 선택
- `nalgaeset gugyeol 261121.txt` 파일을 컴퓨터에 저장

### 1. 제어판 열기

<img width="659" height="546" alt="image" src="https://github.com/user-attachments/assets/0ae2af8e-05b3-4bd2-bc9c-bee3789f78ba" />

- **날개셋 편집기 → 도구 → 날개셋 제어판** 실행
- 왼쪽 **입력기 계층**에서 사용할 입력 항목 선택 (예: `0* 두벌식 옛한글`)


### 2. 사용자 정의 후보 활성화

<img width="662" height="473" alt="image" src="https://github.com/user-attachments/assets/bbcde6d5-e2ab-4fba-afa0-82d4b7a026c4" />

- 왼쪽 **입력기 계층 → 두벌식 옛한글 → 입력 일반** 선택


<img width="662" height="472" alt="image" src="https://github.com/user-attachments/assets/a31ea022-9379-4601-957b-ac36cf407431" />

- **사용자 정의 후보 → 제2 내장형** 체크
- 활성화된 **설정(N)...** 클릭


### 3. 후보 파일 불러오기

<img width="662" height="478" alt="image" src="https://github.com/user-attachments/assets/256f69ef-df16-4b6a-899f-0004d67679b9" />

- **내장형 후보 데이터** 창에서 **가져오기(R)...** 클릭
- 처음에 다운 받은 `nalgaeset gugyeol 261121.txt` 파일 선택
- **확인**을 눌러 후보 데이터 창 닫기


### 4. `Shift+한자` 단축글쇠 확인

<img width="662" height="469" alt="image" src="https://github.com/user-attachments/assets/e6104d21-7769-4572-9cb1-4ef09949101b" />

- 제어판 왼쪽 **편집기 계층 → 단축글쇠** 선택
- 목록에 **`Shift+한자`** 항목이 있는지 확인
- 아래 값으로 설정되어 있는지 확인. 아니면 수정
  - **글쇠:** `Shift+한자`
  - **용도:** `2 낱개선택자 입력`
  - **계산식:** `C0|0x83`

<img width="662" height="487" alt="image" src="https://github.com/user-attachments/assets/6b003c6c-79bb-432d-bb9c-21841d0a9e23" />


### 5. 적용하고 입력하기

- 날개셋 제어판에서 **적용 → 확인** 순서로 저장
- 날개셋 편집기에서 해당 입력 항목 사용
- 원하는 글자(예: `뎌`)를 입력하고 **`Shift+한자`** 누르기
- 표시되는 구결자 후보 중 원하는 문자 선택
- 초성(예: `ㄱ`)을 키로 입력하면 그 초성에 묶어 둔 여러 독음의 구결자 후보를 한꺼번에 확인할 수 있음

![구결자 입력](https://raw.githubusercontent.com/go00ood/gugyeol/main/구결자%20입력.gif)

## 입력기 종합설정 변경

- 날개셋 버전에 따라 구결자 후보 파일을 정상적으로 불러오지 못하는 경우가 있음.
- 이러한 경우를 위해 구결자 후보 데이터가 포함된 **입력기 종합설정 파일(.set)**을 제공함.
- 단, 이 방법은 기존 날개셋 입력 설정 전체를 변경할 수 있으므로, **반드시 자신의 설정을 먼저 백업할 것.**

### 1. 기존 설정 백업

- 날개셋 편집기 → 도구 → 날개셋 제어판 실행
- 왼쪽 아래의 **내보내기** 클릭
- 현재 설정을 `.set` 파일로 저장

### 2. 구결자 종합설정 불러오기
- [날개셋 종합설정 파일](https://github.com/go00ood/gugyeol/blob/main/%EA%B5%AC%EA%B2%B0%EC%9E%90%20%EC%A2%85%ED%95%A9%EC%84%A4%EC%A0%95.set
)에 접속
- 파일 오른쪽 상단의 **Download raw file** 아이콘(<escape>↓</escape>)을 클릭
- `구결자 종합설정.set` 파일 다운로드

- 왼쪽 아래의 **가져오기** 클릭
- 제공된 구결자 종합설정(`.set`) 파일 선택
- 설정을 불러온 뒤 **적용 → 확인** 클릭

<img width="664" height="480" alt="image" src="https://github.com/user-attachments/assets/797333a2-0933-4b79-b16f-e623d70f335e" />

- [재확인](#2-사용자-정의-후보-활성화) 사용자 정의 후보 부분에 잘 저장되어 있는지 확인
- 구결자의 독음이나 초성을 입력한 후 **Shift+한자**를 눌러 후보가 표시되는지 확인
<img width="664" height="475" alt="image" src="https://github.com/user-attachments/assets/07e7487f-5ac6-4cad-a282-ac5a081f68e2" />

※ 이 방법은 버전 차이로 후보 데이터를 가져오지 못하는 경우를 위한 임시 대안. 종합설정 파일 역시 날개셋 버전에 따라 호환되지 않을 수 있으며, 불러오기에 성공하더라도 기존 글쇠배열과 단축글쇠 설정이 변경될 수 있음.

