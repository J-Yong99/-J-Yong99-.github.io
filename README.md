# git-hub.io build 과정

1. j-yong99.github.io로 repository 생성

![1](https://user-images.githubusercontent.com/77261304/203537869-3deae9ff-c02a-4756-a17c-9b73d03b7158.png)


1. index.html이랑 [read.md](http://read.md) 추가
![2](https://user-images.githubusercontent.com/77261304/203537974-f292334f-2cdc-4286-b390-788a31adac97.png)

![3](https://user-images.githubusercontent.com/77261304/203538130-f4a49326-8276-4e34-9f3d-d3704993df8c.png)


1. ruby와 jekyll설치
    - rvm을 설치하고 rvm을 이용해 ruby2.6.6을 설치했다.
    - 그 후 jekyll을 설치했다.
    - 맥OS에서 rvm을 이용한 ruby다운로드 과정에서 힘든 과정이 있었다.
    ![4](https://user-images.githubusercontent.com/77261304/203538211-93e1c7db-e681-4404-a6bc-6876a6b3c2b4.png)
    ![5](https://user-images.githubusercontent.com/77261304/203538301-0b5bc87e-a1ad-4501-8acd-537fcbb433e2.png)





    
2. 그 후 jekyll을 시작해보자
    ![6](https://user-images.githubusercontent.com/77261304/203538541-8a958f8e-912d-457c-9e88-fa3704f96b39.png)
    ![7](https://user-images.githubusercontent.com/77261304/203538553-c03ed22e-e861-43dc-81e5-c3029fd363f0.png)
    ![8](https://user-images.githubusercontent.com/77261304/203538567-5c398320-273e-4a32-821d-964caefad62f.png)
    
    성공!!
    
3. 9번의 시도 후에 기본테마의 지킬 블로그를 깃헙블로그와 연동해 j-yong99.github.io 로 접속 시 연결된다.
![9](https://user-images.githubusercontent.com/77261304/203538673-77116624-54a4-4386-bbb2-1bd3691c527b.png)


[](http://j-yong99.github.io)

1. post 올리기
    - 매우 엄청나게 오랜 시행 착오 끝에 성공
    ![1](https://user-images.githubusercontent.com/77261304/203560806-18bfacb0-4bed-441c-ad1d-ac5ad14756f0.png)

    ![2](https://user-images.githubusercontent.com/77261304/203560909-e4135d81-7448-4ded-87c2-7ce04fbc65e1.png)
    
2. 테마 입히기
    - 일단 테마를 가져와서 적용했더니 많은 것이 바뀌었고 데모 버전에 맞게 다양한 요소들을 추가해줬다
       
    ![3](https://user-images.githubusercontent.com/77261304/203561067-76d30201-2616-4d90-931e-48240fe369e8.png)
    
    - 상단바와 하단바도 추가하고 고쳐주었다.
        
    ![4](https://user-images.githubusercontent.com/77261304/203561585-70e4295c-5adf-4bbe-b497-268425251ae7.png)

        
3. post하기
    - 노션에서 작업한 마크다운 파일을 다운로드 받은 후 _post디렉토리에 넣어준다.
    - 사진 같은 경우 asset directory에 넣어주고 노션에서 작업한 마크다운 파일을 서식에 맞게 바꿔준다.
    
    ![5](https://user-images.githubusercontent.com/77261304/203561704-b685385a-59bb-420e-82c8-ffc799bab028.png)

    ![6](https://user-images.githubusercontent.com/77261304/203561767-3485eabf-75b1-45b1-a496-5654174cda76.png)
    
4. 댓글 기능 추가
    - disqus를 이용한 댓글 기능을 추가했다.
    - 상당히 많은 시간이 걸렸다.
    
    ![7](https://user-images.githubusercontent.com/77261304/203561843-8d5b0982-e9fc-4e0d-b897-db94fc0f6d33.png)

5.  Google analytics 추가
    - 구글 애널리틱스에 계정을 추가하고 스트림을 추가한다.
    - 그리고 config파일을 수정해주면 된다.
    ![8](https://user-images.githubusercontent.com/77261304/203562033-d265f8fb-fe6d-4431-af59-de02de85cfa8.png)

    ![9](https://user-images.githubusercontent.com/77261304/203562043-f98eafc4-a3d5-4a84-b12e-4509016b18f3.png)

9. favicon 설정

- favicon은 위에 뜨는 사이트 이모티콘인데 원하는 이모티콘을 다운 받은 후

![10](https://user-images.githubusercontent.com/77261304/203562161-36691803-d7e2-4c2a-944c-3c1f730c81ac.png)


- 파란색 집모양을 다운받았다.
- 다운받은 icon들은 전부 assets/img디렉토리에 넣어주고

![11](https://user-images.githubusercontent.com/77261304/203562182-ab62b358-b447-40e2-8a0e-9ca01838d388.png)

- _includes/head.html에 추가해준다.
![12](https://user-images.githubusercontent.com/77261304/203562272-11fa8ec6-8b5a-4847-b57a-395e1ea37367.png)
![13](https://user-images.githubusercontent.com/77261304/203562233-a40f8ab6-08b2-47ba-b1c6-ac60b877e691.png)
- 이렇게 파란 집이 보인다.
