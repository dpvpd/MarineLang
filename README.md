# 해병언어
MarineLang is a Programming language from Korean Marine literature meme
해병언어는 해병문학과 엄랭([umjunsik-lang][umjunsiklang])에 영감을 받아 고안한 언어입니다. 
2022년 04월 24일 기준 해병언어는 구현체가 없는 아이디어에 불과합니다!

[umjunsiklang]: https://github.com/rycont/umjunsik-lang "엄랭"
```
악! 해 병언어는즐거워 해병님!
해 병언어는즐거워 해병님!
악! 구 구단을외는것은뭐든지잘해 해병님!
구 구단을외는것은뭐든지잘해 새끼.기합! 

따흐흑 병언어는즐거워
따흐흑 새끼..기합! 새끼...기합! 전우애 새끼.......기합! 전우애 실시! 해병님...
따흐흑 구단을외는것은뭐든지잘해
따흐흑 병언어는즐거워 구단을외는것은뭐든지잘해 전우애 실시!
따흐흑 새끼..........기합! 해병님...
구 구단을외는것은뭐든지잘해 구단을외는것은뭐든지잘해 새끼.기합! 악! 실시!
구단을외는것은뭐든지잘해 해서 지고 새끼..........기합! 이면 죽어라!
    새끼.....기합! 하였으니 참으로 기쁜 일이 아닐 수 없지 않은가!
여간 기합이 아니었다.
```

# 문법
## 주의! 해병언어는 보는 이가 불편할 수 있는 내용을 포함합니다. 
### 본 글의 작성자는 순수한 의도로만 해병언어를 고안했으며, 다소 선정적으로 보인다면 작성자가 아닌 귀하의 사고방식에 무언가 문제가 있음을 의미합니다. 
모든 해병언어 코드는 "여간 기합이 아니었다."로 끝나야합니다.
해병언어는 "악!", "새끼", "기합!", "기열!", "해병님", "따흐흑", "전우애", "실시!", "하였으니 참으로 기쁜 일이 아닐 수 없지 않은가!", "해서 지고", "이면 죽어라!" 라는 11개의 키워드와 "!", ".", "…" 세개의 기호로 코드가 이루어집니다. 단, "…"기호의 경우 코드작성의 편의성을 위해 "..."으로 작성하는 것을 허용합니다. 

## 주석
"라이라이차차차" 또는 "헤이빠"와 "빠리빠"로 주석처리를 할 수 있습니다.
각각 C언어의 ```//```, ```/*```, ```*/```에 대응됩니다. 
```
라이라이차차차 이 부분은 한 줄짜리 주석입니다. 
헤이빠
이 부분은
여러 줄
주석입니다.
빠리빠
```

## 자료형
정수 : "새끼", ".", "기합!", "기열!"로 표현합니다. "새끼"로 시작하여 "기합!"의 경우 "."의 개수만큼의 정수를 의미하며, "기열!"의 경우 "."의 개수만큼의 음의 정수를 의미합니다. 
```
새끼...기합! => 3
새끼..기합! => 2
새끼..기열! => -2
새끼...기열! => -3
새끼기합! => 0
새끼기열! => 0
```

## 연산자
* 덧셈: ```악!```
* 뺄셈: ```따흐흑```
* 곱셉: ```전우애```

해병언어의 연산식은 후위표기식을 따릅니다. 또한, 모든 계산식의 끝에는 "실시!"를 써 연산식이 끝났음을 알립니다. 
```
새끼...기합! 새끼...기합! 악! 실시! => 3+3 = 6
새끼...기합! 새끼..기합! 따흐흑 실시! => 3-2 = 1
새끼.....기합! 새끼..기열! 악! 실시! => 5 + (-2) = 3
새끼...기합! 새끼....기합! 전우애 실시! => 3 * 4 = 12
새끼..기합! 새끼...기열! 전우애 실시! => 2 * (-3) = (-6)
```

## 변수
모든 변수는 정수형 변수입니다. 
### 선언
변수는 "악! (접두어) (변수이름) 해병님!"의 형태로 선언합니다. 
```
악! 해 병언어는즐거워 해병님! => "병언어는즐거워" 라는 변수를 선언
악! 프 로그램을만드는것은뭐든지잘해 해병님! => "로그램을만드는것은뭐든지잘해" 라는 변수를 선언
```
### 대입
변수에 값을 대입하기 위해선 변수를 선언할 때 사용한 접두어와 변수 이름을 "(접두어) (변수이름)" 형태로 작성합니다. 변수이름 뒤에 오는 값을 해당 변수에 대입합니다. 이 때, 한 변수에 대한 접두어는 여럿이 될 수 있으며 반드시 한 글자여야합니다. 
```
악! 해 병언어는즐거워 해병님! => "병언어는즐거워" 라는 변수를 선언
해 병언어는즐거워 새끼...기합! => "병언어는즐거워"변수에 3을 대입
공 병언어는즐거워 새끼..기합! => "병언어는즐거워"변수는 접두어 "공"과 함께 선언되지 않았으므로 오류 발생
```
```
악! 해 병언어는즐거워 해병님! => "병언어는즐거워" 라는 변수를 선언
악! 공 병언어는즐거워 해병님! => "병언어는즐거워"변수의 접두어로 "해" 외에도 "공"을 사용하겠음을 명시함.
해 병언어는즐거워 새끼...기합! => "병언어는즐거워"변수에 3을 대입
공 병언어는즐거워 새끼..기합! => 3의 값을 갖고있던 "병언어는즐거워" 변수에 2의 값을 새로 대입
```
### 사용
변수 이름을 그대로 작성합니다. 
```
악! 해 병언어는즐거워 해병님! => "병언어는즐거워" 라는 변수를 선언
악! 코 드를짜는것은뭐든지잘해 해병님! => "드를짜는것은뭐든지잘해" 라는 변수를 선언
해 병언어는즐거워 새끼...기합! => "병언어는즐거워"변수에 3을 대입
코 드를짜는것은뭐든지잘해 병언어는즐거워 새끼.....기합! 전우애 실시! => "드를짜는것은뭐든지잘해"변수에 "병언어는즐거워"에 저장된 3과 5를 곱한 값을 대입
```

## 콘솔
### 해병님!
콘솔에서 정수를 입력받습니다.
```
악! 해 병언어는즐거워 해병님! => "병언어는즐거워" 변수를 선언합니다. 
해 병언어는즐거워 해병님! => "병언어는즐거워" 변수에 입력받은 정수값을 대입합니다.
라이라이차차차 
```

### 따흐흑
콘솔에 정수를 출력합니다. 
