# Expect 예제 코드들입니다.

## sshConnect.exp
Expect의 기본 문법인 tcl로 구현한 ssh 로그인을 수행하는 코드입니다.
### 실행
> sshConnect.exp [host] [userId] [password]

## sshConnect.pl
Perl의 Expect 모듈을 이용하여 구현한 ssh 로그인 수행 코드입니다.
> sshConnect.pl [host] [userId] [password]

## sshConnectUseNetSSHExpect.pl
Perl의 Expect의 확장 모듈인 NetSSHExpect를 이용하여 구현된 SSH 로그인 수행 코드입니다.
[[출처]](https://metacpan.org/pod/distribution/Net-SSH-Expect/lib/Net/SSH/Expect.pod)  
> sshConnectUseNetSSHExpec.pl

## commandExpect.pl
Perl의 Expect 모듈을 이용하여 원격으로 로그인 후 입력된 명령을 수행하는 코드입니다.  
> commandExpect.pl -h [host] -u [userId] -p [userPassword] -rp [host's root password] -C [Command String]
#### Options
  - -F [filePath] : 파일 모드로 수행. filePath는 원격에서 실행할 명령어 파일
  - -C [commandString] : 명령어 모드로 수행. 
  - -S : SSH로 접속
  - -T : Telnet로 접속
  - -P [Port] : 원격 접속할 포트 번호
