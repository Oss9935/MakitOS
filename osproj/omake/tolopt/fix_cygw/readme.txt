doscmd(copy.exe와 del.exe)에 대해 카와이 히데미

[이것은 뭐지? ]

  doscmd는, Cygwin를 인스톨 하면 copy 커맨드나 del 커맨드를 사용할 수 없게
되어 버린다고 하는 중대한 문제(장해라고 해도 괜찮을지도)를, 어떻게든 해 해결하기 위해서
개발되었습니다. copy.exe나 del.exe의 내용은 doscmd.exe와 완전히 같습니다.

  doscmd는 파일명을 바꾸면 그 커맨드로 「바뀌게」됩니다. 예를 들어 copy.exe로
하면 DOS prompt의 copy 커맨드 대신이 됩니다. 뭐 tolset를 사용하는 분들은
여기에 들어가 있는 copy.exe와 del.exe만 있으면 우선 부자유스럽지는 않을 것입니다.

  즉, Cygwin를 사용하지 않은 사람은 이런 소프트웨어를 사용할 필요는 전혀 없습니다. 이런
것은 잊어 버립시다!

  이 아카이브(archive)의 라이센스는 KL-01입니다.

[사용 방법]

  이 폴더 안의 copy.exe와 del.exe를, 예를 들어 C:\WINDOWS에 카피합니다
(이것이 없으면 C:\WINNT일지도 모릅니다). 이것으로 아마 Cygwin의 파일보다 우선
으로 이 copy.exe나 del.exe가 실행되게 되고, 「하리보테 OS」의 Makefile이
수정 되지않아도 정상 동작할 것입니다. 감사, 감사.

  상기로 잘 되지 않는 경우, 이 copy.exe나 del.exe를 어디에 카피하면 좋은가는
path 커맨드를 실행하여 폴더의 우선도를 확인하고, 가능한 한 우선 순위가 높은 곳
에 놓으면 효과가 있다고 생각합니다.

[상급자전용]

  doscmd는 파일명을 바꾸지 않아도, 다양한 내장 커맨드를 실행할 수 있습니다.
예를 들면 이런 식으로.

prompt>doscmd --dir a:\

포인트는 최초로 --커맨드명을 붙인 것입니다.

  뭐 동일한 점은 cmd.exe /C dir a:\ 등으로 하면 할 수 있습니다만, doscmd를 사용하면
Win9X계에서도 WinNT계에서도 동일한 표현으로 쓸 수 있으므로 조금 편리할지도 모릅니다.
