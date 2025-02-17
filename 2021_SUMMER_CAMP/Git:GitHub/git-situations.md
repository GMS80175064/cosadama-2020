# 깃 실습 시현

오이카와 : administrator 프로젝트 메인 진행자, 레포지토리 권한 O - 가윤
스가와라 : collaborator 프로젝트 서브 진행자, 레포지토리 권한 O - 정윤
히나타 : contributer 프로젝트 기여자, 레포지토리 권한 X - 용주

### 배경 설명
여기 오이카와와 스가와라라는 고등학교 3학년의 두 친구가 있습니다. 두 친구는 19년 최고 성적을 낸 배구 선수들을 분석해보려 해요. 오이카와가 제안한 프로젝트이기 때문에 작업 중간중간 스가가 도움을 주는 방식으로 진행하기로 했어요.

### 오이카와 작업 시나리오 #1
오이카와는 자신이 준비해둔 데이터인 19년 배구 선수 데이터와 분석 초안 파일을 가지고 있어요. 스가와의 협업을 위해서는 해당 작업 폴더에 깃을 설치하고 온라인 저장소에 올려줘야겠죠?

1. 로컬 폴더에 깃 설치하기 (git init) : 오이카와의 로컬 폴더(Working Directory)에는 csv 파일과 ipynb 파일이 있어요. 해당 파일들의 변화를 추적해줄 git을 설치해봅시다.
2. 깃헙 레포지토리 만들기 : 스가와라와의 협업을 위해 클라우드 저장소가 필요하겠죠? 깃헙에 온라인 프로젝트 저장소인 레포지토리를 만들어봅시다.
3. 로컬 폴더와 레포지토리 연결하기 (git remote add) : 로컬 폴더의 변화들을 모아 온라인 레포지토리에 커밋하기 위해 로컬 폴더와 레포지토리를 연결시켜줘야겠죠?
4. 커밋에 포함할 변화 고르기 (git add) : 커밋은 ‘의미있는 변화의 덩어리’라고 했어요. 커밋하기 전, 덩어리에 포함시킬 변화를 골라 스테이지 공간에 올려두는 게 필수라고 했죠? git add를 통해 변화들을 골라봅시다.
5. 고른 변화들을 덩어리로 묶어주기 (git commit) : git add를 통해 스테이지 공간에 있는 변화들을 덩어리로 묶어줘야 해요. 이 덩어리들이 레포지토리에 입력이 되면, 이제 이 커밋 자체가 새로운 버전이 됩니다.
6. 커밋을 레포지토리에 적용하기 (git push) : 커밋을 레포지토리에 적용하는 일반적인 방법이에요. 커밋 적용, 즉 푸쉬 전후로 버전이 달라집니다.

### 스가와라 작업 시나리오 #1
오이카와의 작업물을 받아와서 작업을 해야하는 스가와라, 어떻게 프로젝트를 진행할까요?

1. 공개된 레포지토리 로컬 폴더에 받기 (git clone) : 오이카와의 레포지토리를 로컬 폴더에 다운받아줄 거에요! 주의할 점은, 특정 폴더 내에서 clone할 경우 뒤에 . 을 붙여줘야 한다는 점!
2. 작업하기 : 스가와라는 세터 포지션이기 때문에 세터 선수들만 따로 빼내어 데이터프레임을 만들었어요.
3. 커밋에 포함할 변화 고르기 (git add)
4. 고른 변화들을 덩어리로 묶어주기 (git commit)
5. 커밋을 레포지토리에 적용하기 (git push)

### 오이카와 작업 시나리오 #2
앗 스가와라가 작업을 시작했네요! 레포지토리에 적용된 스가와라의 커밋을 로컬 폴더에도 적용시켜줄게요.

1. 레포지토리의 커밋 로컬 폴더에 적용하기 (git pull) : 스가와라의 커밋을 로컬 폴더에 적용시켜줄 거에요. 이를 위해서는 git pull이라는 명령어를 사용합니다. git pull origin도 가능하고, git pull [repository URL]도 가능해요. 적용 완료!

### 히나타 작업 시나리오#1
순조롭게 진행이 되는 것 같았는데 1학년 히나타가 들어왔어요. 히나타는 아직 배운 게 적고 실수가 많아 오이, 스가처럼 직접 푸쉬를 하는 건 위험할 것 같아요. 위험성을 줄이기 위해 히나타는 포크를 통해 자신의 깃헙 계정에 복사본 레포지토리를 만들고, 복사본 레포지토리에 커밋 및 푸쉬를 한 후 해당 변화를 오리지널 레포지토리에 적용하기로 했어요.

1. 클라우드 서비스에 레포지토리 복사본 만들기 (fork repository) : 오이카와, 스가와라 선배들에 비해 경험이 부족해 실수할 가능성이 많은 히나타! 위험을 줄이기 위해 복사본을 만들어 작업할 거에요. 레포지토리 복사본을 만드는 방법은 fork repository입니다.
2. 공개된 레포지토리 로컬 폴더에 받기 (git clone)
3. 작업하기 : 히나타는 최고의 선수들을 랭킹 순으로 나열해보고 싶어요. 높은 점수의 선수가 롤 모델!
4. 커밋에 포함할 변화 고르기 (git add)
5. 고른 변화들을 덩어리로 묶어주기 (git commit)
6. 커밋을 레포지토리에 적용하기 (git push)
7. 오리지널 레포지토리에 적용 위해 풀리퀘 열기 (open pull request) : 히나타가 푸쉬한 커밋은 복사본 레포지토리에 적용됐어요. 이 커밋을 오리지널 레포지토리에도 적용하기 위해서는 레포지토리에 access를 가진 선배들이 직접 병합시켜줘야 해요. 선배들에게 커밋 병합을 요청하는 것이 바로 pull request에요.

### 스가와라 작업 시나리오 #2
히나타의 커밋 요청(pull request)을 받아들여 오리지널 레포지토리에 적용해주고(merge), 새로운 작업을 업로드 하려 해요.

1. 풀리퀘 오리지널 레포지토리에 병합하기 (merge) : 히나타의 풀리퀘(pull request)를 보니 충돌하는 등의 에러는 없는 것 같아요. 오리지널 레포지토리에 병합해 줄게요.
2. 작업하기 : 히나타의 작업물인 랭킹 세우기를 보니, 스가와라도 세터 선수들을 랭킹으로 세워보고 싶어요. 이전에 만든 세터 데이터프레임에서 랭킹 순으로 나열해 볼게요.
3. 커밋에 포함할 변화 고르기 (git add)
4. 고른 변화들을 덩어리로 묶어주기 (git commit)
5. 커밋을 레포지토리에 적용하기 (git push)

### 히나타 작업 시나리오 #2
스가와라 선배가 새로 커밋을 올렸다고 해요! 복사본 레포지토리를 업데이트해주고, 로컬 폴더도 업데이트 해줘야겠어요.

1. 오리지널 레포지토리 커밋 받아오기 (fetch and merge) : 오리지널 레포지토리에 적용된 스가와라 선배의 새로운 커밋을 복사본 레포지토리에도 받아와 복사본을 최신으로 유지해줍니다!
2. 레포지토리의 변화 로컬 폴더에 적용하기 (git pull)








