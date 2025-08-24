# Todo-Green
사용 기술: React , Tailwind Css
<img width="1803" height="750" alt="image" src="https://github.com/user-attachments/assets/276d2d38-9ef5-47bb-b90a-06d5b5c4777d" />

**컴포넌트를 여러 개 가져옴:**

**1. ProjectsSidebar : 왼쪽에 프로젝트 목록을 보여주고 선택할 수 있는 사이드바.**

**2. NewProject : 새로운 프로젝트 생성 폼.**

**3. NoProjectSelected: 프로젝트가 선택되지 않았을 때 보이는 화면.**

**4. SelectedProject : 선택된 프로젝트 상세 화면(삭제, 할 일 추가/삭제 포함).**

## React의 useState 훅을 사용.

<img width="602" height="154" alt="image" src="https://github.com/user-attachments/assets/d2b67f3e-cfc0-4ea5-84eb-47fd0889611e" />

+ projectsState라는 상태를 하나로 묶어서 관리:
  + selectedProjectId: 현재 선택된 프로젝트의 id
    + undefined: 아무 프로젝트도 선택되지 않은 상태.
    + null: 새 프로젝트 추가 모드.
    + id값: 특정 프로젝트가 선택된 상태.
  + projects: 프로젝트 목록 배열.
  + tasks: 작업(Task) 목록 배열.

## Task 관련 함수
<img width="508" height="363" alt="image" src="https://github.com/user-attachments/assets/a20ac1c3-0b8d-4b14-a0d3-3c57f95a0b01" />

+ 현재 선택된 프로젝트(selectedProjectId) 안에 새 작업을 추가.
+ Math.random()으로 임시 id 부여.
+ 기존 tasks 배열 앞에 새 task를 추가.

<img width="679" height="207" alt="image" src="https://github.com/user-attachments/assets/eb9a1183-8c83-4c06-86d1-aae3b7c13ccd" />

+ 특정 task를 삭제 (filter 사용).

## Project 선택 관련 함수
<img width="506" height="211" alt="image" src="https://github.com/user-attachments/assets/f81eabc5-afb4-49f0-89be-c2245bba6986" />
+ 사이드바에서 프로젝트를 선택했을 때 호출.
+ selectedProjectId를 해당 id로 바꿈.

## Project 추가 모드/취소 함수
<img width="418" height="207" alt="image" src="https://github.com/user-attachments/assets/dafca70a-9529-44e8-9f69-cd1ec2244b2b" />

+ 프로젝트 추가 버튼을 눌렀을 때 실행.
+ selectedProjectId를 null로 바꿔서 "새 프로젝트 폼"을 보여주게 함.

<img width="412" height="213" alt="image" src="https://github.com/user-attachments/assets/7865551c-3a9f-41b0-b213-a8d10043490b" />

+ 프로젝트 추가 취소 → 다시 아무것도 선택되지 않은 상태로 변경.

## Project 추가 & 삭제 함수
## 현재 선택된 프로젝트 가져오기
## 최종 반환
<img width="608" height="253" alt="image" src="https://github.com/user-attachments/assets/fc043bb4-dd7f-4faa-ac33-a4adcf1bde1c" />

<img width="1312" height="641" alt="image" src="https://github.com/user-attachments/assets/04eea6f3-d0b7-4ebb-912c-854a11aceb22" />
<img width="1000" height="592" alt="image" src="https://github.com/user-attachments/assets/015f10eb-9a3e-4e8c-bfec-62a725a45d32" />
<img width="1182" height="672" alt="image" src="https://github.com/user-attachments/assets/16beae2f-3df4-48c0-9544-fa41931962a6" />
