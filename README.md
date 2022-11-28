# B4AFTER_Deeplearning_Backend

# 프로젝트 개요

### 프로젝트 명 : montmartre(몽마르트)

- 세계적으로 유명한 화가 고흐가 실제로 살았었던 프랑스의 몽마르뜨 언덕은 지금도 예술가들의 본거지라는 평가를 받고 있다. 이러한 몽마르뜨 언덕 위의 화가가 원하는 이미지를 세계 유명화가들의 화풍으로 그려주는 사이트를 구상해보았다.

## 목표

- 이미지를 업로드하면 해당 이미지를 세계 유명 화가들의 화풍으로 변환하고 변환된 이미지를 사용자에게 제공한다.
- 사용자는 제공받은 이미지를 사이트 내의 커뮤니티에 올려 다른 사용자와 공유할 수 있고 다른 사용자들의 이미지에 댓글을 남길 수 있다.


## 주요 구현 기능

## Wireframe

[https://www.figma.com/embed?embed_host=notion&url=https%3A%2F%2Fwww.figma.com%2Ffile%2F4fjn58rEJAKCAKfw4ZPuxY%2FB4AFTER-ML%3Fnode-id%3D0%253A1%26t%3DyIBwdpS7CtxxV21U-1](https://www.figma.com/embed?embed_host=notion&url=https%3A%2F%2Fwww.figma.com%2Ffile%2F4fjn58rEJAKCAKfw4ZPuxY%2FB4AFTER-ML%3Fnode-id%3D0%253A1%26t%3DyIBwdpS7CtxxV21U-1)

### 페이지 관계성

![relation.PNG](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8cdd08f2-dbe0-4a94-b8a3-c01839ba8529/relation.png)

- 로고 버튼 클릭 시 메인페이지로 이동
- 메인 페이지 내에 게시된 이미지 클릭 시 댓글을 달 수 있는 상세페이지로 이동
- 로그인 버튼 클릭 시 로그인 페이지로 이동
- 로그인 완료 시 메인페이지로 이동
- 로그인 창에서 회원가입 버튼 클릭 시 회원가입 페이지로 이동
- 회원가입 창에서 회원가입 완료 시 로그인 페이지로 이동
- 우측 상단 로그인 버튼은 로그인 시 로그아웃 버튼으로 변경, 로그아웃하면 다시 로그인으로 변경

## 로그인

![login.PNG](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6627dc06-6944-46a3-bdff-a99b9856fd4c/login.png)

- DB에 저장된 username과 password를 비교하여 일치하지 않으면 오류 알림
- 만약 username이나 password가 빈칸으로 작성되었다면 오류 알림
- 회원가입 버튼 클릭 시 회원가입 페이지로 이동
- 로그인 완료 시 메인 페이지로 이동

## 회원 가입

![signup.PNG](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/47f1a6b8-40aa-4db6-8d8e-d3729a4135ee/signup.png)

- 로그인이 되어있지 않을 때만 회원 가입 페이지로 이동 가능
- 비밀번호와 비밀번호 확인이 일치하지 않으면 오류 알림
- 중복된 username 존재 시 오류 알림
- 회원 가입 완료 시 로그인 페이지로 이동

## 이미지 생성 기술

![main.PNG](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/abab38c5-685c-4642-8861-5baeb46dbcdb/main.png)

- 이미지를 업로드 하고 스타일을 선택하면 해당 스타일에 맞도록 이미지를 변환하고 결과물 제공
- 제공된 이미지를 사이트 내 커뮤니티에 공유 가능
- (추가 기능) 제공된 이미지를 인스타그램, 페이스북 등 외부 SNS에 공유 가능

## 생성된 이미지 공유(게시글)

![detail.PNG](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/cf42d90e-cd42-428b-810d-56f26ca89a29/detail.png)

- 생성된 이미지를 사이트 내 커뮤니티에 게시
- (추가 기능) 타인이 작성한 게시글에 댓글 남기기 가능
- (추가 기능) 타인이 작성한 게시글에 좋아요 남기기 가능

# DATABASE 구조(흐름)APP(단위) 기능

[https://www.erdcloud.com/p/ji5u4nHoRz2dRZfMA](https://www.erdcloud.com/p/ji5u4nHoRz2dRZfMA)
