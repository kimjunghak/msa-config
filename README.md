# msa-config
msa config


## 오류상황
1. spring cloud config 공식 페이지에 보면   

    ```http request
   /{application}/{profile}[/{label}]
    /{application}-{profile}.yml
    /{label}/{application}-{profile}.yml
    /{application}-{profile}.properties
    /{label}/{application}-{profile}.properties
   ```
    해당 엔드포인트가 제공된다고 한다. 이 형식에 맞춰 파일 수정
2. spring.profiles={profile}을 config-server 에서 읽지 못한다.
   spring.activate.on-profile: {profile} 로 변경