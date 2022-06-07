# 모바일컴퓨팅 프로젝트
<hr></hr>

## 안드로이드 코딩 강좌의 TodoList를 만들어봤습니다.<br>

SqlLite 대신 Room 라이브러리를 이용해서 제작했습니다<br>

DAO( @Query를 사용)로 Sql Select문을 이용한 정렬기능을 구글에서 찾아보고 구현했습니다<br>

하단의 EditText에 내용을 입력 후 '추가' Button을 누르면 viewModel객체 내의 MutableLiveData의 value의 값이 변경되도록 설정했습니다.<br>

CheckBox 체크 시 isChecked의 값을 todo.isDone 넣어주고, todo.isDone의 값에 따라 취소선(-)이 표시되게 하였습니다<br>

'X'버튼을 통해 삭제하거나 menu의 완료 삭제를 통해 삭제를 합니다. todoDao의 delete 메서드를 통해 삭제하는 방식으로 진행하였습니다.<br>

등록하는 순간 System의 시간을 받으므로 등록일 순 정렬에 사용할 기준이 됩니다.(이를 통해 시간순으로 정렬할 수 있습니다)<br>
