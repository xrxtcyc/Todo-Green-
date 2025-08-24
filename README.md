# Todo-Green
사용 기술: React , Tailwind Css
<img width="1803" height="750" alt="image" src="https://github.com/user-attachments/assets/276d2d38-9ef5-47bb-b90a-06d5b5c4777d" />
## React의 useState 훅을 사용.

컴포넌트를 여러 개 가져옴:

ProjectsSidebar: 왼쪽에 프로젝트 목록을 보여주고 선택할 수 있는 사이드바.

NewProject: 새로운 프로젝트 생성 폼.

NoProjectSelected: 프로젝트가 선택되지 않았을 때 보이는 화면.

SelectedProject: 선택된 프로젝트 상세 화면(삭제, 할 일 추가/삭제 포함).


const [projectsState, setProjectsState] = useState({
    selectedProjectId: undefined,
    projects: [],
    tasks: [],
  });
projectsState라는 상태를 하나로 묶어서 관리:

selectedProjectId: 현재 선택된 프로젝트의 id.

undefined: 아무 프로젝트도 선택되지 않은 상태.

null: 새 프로젝트 추가 모드.

id값: 특정 프로젝트가 선택된 상태.

projects: 프로젝트 목록 배열.

tasks: 작업(Task) 목록 배열.
<img width="1312" height="641" alt="image" src="https://github.com/user-attachments/assets/04eea6f3-d0b7-4ebb-912c-854a11aceb22" />
<img width="1000" height="592" alt="image" src="https://github.com/user-attachments/assets/015f10eb-9a3e-4e8c-bfec-62a725a45d32" />
<img width="1182" height="672" alt="image" src="https://github.com/user-attachments/assets/16beae2f-3df4-48c0-9544-fa41931962a6" />
