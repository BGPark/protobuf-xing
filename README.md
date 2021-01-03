# protobuf-xing
protocol buffer definitions for XingAPI system trading

# 파이썬용 생성하기
protoc.exe --python_out=.\ xing.proto

# Note.
프로토콜 버퍼 신택스에서는 모두 lowcase와 언더스코어가 제거됩니다. 애석하게도 Xing의 RES에서 해당 부분에 의한 컨플릭트가 발생하여 몇군데 수정이 되었습니다.
* 언더 스코어는 '9'로 치환되었습니다.
* userId 와 userid가 중복으로 두 번째는 userIdOrder로 치환되었습니다.
