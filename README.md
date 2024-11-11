

# 4주차 편의점 미션 코레아에서 코드 리뷰하는 방법

## [1] 저장소를 공개로 변경하기

깃허브 저장소 오른쪽 상단에 있는 Settings를 클릭합니다.

제일 하단의 "Danger Zone"으로 스크롤합니다.

"Change visibility" > "Change to public" 버튼을 클릭한 뒤 절차를 끝까지 따릅니다.

![3](https://github.com/user-attachments/assets/cd41a55c-e7f6-4d45-bf2f-39693079b8ea)

<br>
<br>

## [2] 본인 레포로 PR 날리기

### 1. 최초 커밋의 해시를 찾습니다.

```bash
git log
```

또는

깃허브에서 "{커밋 개수} Commit" 클릭

![1](https://github.com/user-attachments/assets/da3c2fe5-a330-42ab-8290-98f6897bc1ee)
![2](https://github.com/user-attachments/assets/8db6d962-4fa8-4a1e-a992-079271da598c)

<br>

### 2. 새 브랜치를 생성하며 체크아웃합니다.

위에서 찾은 해시값을 `12345`라고 하면 아래의 명령어를 통해 새로운 브랜치를 생성할 수 있습니다.

```bash
git checkout -b {브랜치 이름} {해시넘버}
```

예시) `git checkout -b corea 12345`

<br>

### 3. 원격 저장소에 푸시합니다.

```bash
git push origin {브랜치 이름}
```

예시) `git push origin corea`

<br>

### 4. Pull requests를 제출합니다.

Pull requests 메뉴에서 `review ← main` 방향으로 PR을 제출합니다.
