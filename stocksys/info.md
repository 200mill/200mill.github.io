# Information
이 Text는 예정된 작업과 확인된 문제, 그에 대한 해결방안등을 서술한 Text입니다.
## Infomration.2
이 Text가 2000자를 넘으면 Web으로 이전시킬겁니다
## 기타 자세한 정보
**None**

# 확인된 문제
## /balance
### 문제 1(planned, 계획됨)
내용 전문:
```
Microsoft.CSharp.RuntimeBinder.RuntimeBinderException: Cannot convert null to 'int' because it is a non-nullable value type
   at CallSite.Target(Closure, CallSite, Object)
   at System.Dynamic.UpdateDelegates.UpdateAndExecute1[T0,TRet](CallSite site, T0 arg0)
   at Example.Modules.StockModule.balance(SocketGuildUser user) in E:\DiscordBot\src\Modules\StockModule.cs:line 289Microsoft.CSharp.RuntimeBinder.RuntimeBinderException: Cannot convert null to 'int' because it is a non-nullable value type
   at CallSite.Target(Closure, CallSite, Object)
   at System.Dynamic.UpdateDelegates.UpdateAndExecute1[T0,TRet](CallSite site, T0 arg0)
   at Example.Modules.StockModule.balance(SocketGuildUser user) in E:\DiscordBot\src\Modules\StockModule.cs:line 289
```
#### 해석
**Microsoft.CSharp.RuntimeBinder.RuntimeBinderException: Cannot convert null to 'int' because it is a non-nullable value type** >> null을 int로 변환할수 없음
#### 원인
Excel CSA처리부분에 0안적어둠(빈칸이라 null이됨)
#### 해결방안
**엑셀만 수정하면됨**
## /withdraw
### 문제 1(not planned, 계획되지 않음)
#### 원인
확인해야함
#### 해결방안
원인 확인후 해결예정
## /addaccount
### 문제 1(not palnned, 계획되지 않음)
내용 전문
```System.Exception: Sucess
   at Example.Modules.StockModule.addaccount(Int64 id, SocketGuildUser user) in E:\DiscordBot\src\Modules\StockModule.cs:line 59```
#### 원인
**Success 처리를 빨리 끝내기 위해 예외를 던지는걸로 함**
#### 그로인한 피해ㅐ
**Fail과 같은 Error로 처리되어 Console이 더러워짐**
#### 해결방안
실행성공 embed로 처리하고 Console에 출력하지 않음
## /userid
### 문제 1(not planned, 계획되지 않음)
#### 원인
**Timeout**
#### 해결방안
**찾을예정**
## /buy
### 문제 1(working, 작업중)
#### 원인
아직 작업 안끝남
#### 해결방안
작업끝나면됨
## /sell
### 문제 1(`planned, but unavailable to work`, `계획되었지만 작업할수 없음`)
#### 원인
buy 작업중이라 sell작업 처리불가
#### 해결 방안
buy작업 완료시 가능

# 기타정보
Developer : @200mill 
Bot : @Stock System#8916 
Bot Online Time : On Debug(디버그중)
Planned T: 0
