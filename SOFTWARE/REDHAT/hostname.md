REDHAT9 버전부터 FC 952 / RFC 1123 호스트명 규격상 허용되지 않는 문자로 hostnamectl set-hostname <hostname> 으로 _ 특수문자 반영이 안됨

hostnamectl status 확인 시 systemd가 자동으로 정규화하여 static hostname과 pretty hostname이 다름<br>
<img src="../../EOS/images/HostnameStatus.png" alt="호스트네임" width="350"><br>

등록 방법: /etc/hostname에 직접 등록<br>
재기동 없이 등록하는 방법: /proc/sys/kernel/hostname에 hostname 입력