# Text to html

사용자 입력(text)에 맞는 html 코드 출력

## 설치 방법

pip install openai

openai API key를 발급받은 다음 API key를 입력해야 합니다.

## 개발환경

google colab

## 내용

1. 배경이미지 생성
   사용자 입력 + 웹사이트 생성을 필요로한 정보를 dall-e-3 모델에 query를 보내 배경이미지 생성
   dall-e-3 모델의 경우 영어 외에 타 언어도 지원하기 때문에 사용. (성능만 보면 영어 입력이 더 좋습니다.)
   
2. html 생성
   사용자 입력 + 웹사이트 생성을 필요로한 정보를 gpt-3.5-turbo 모델에 query를 보내 배경이미지 생성

## 주의사항
dall-e-3 생성된 이미지 url을 그대로 사용하기 때문에 시간이 지나면 해당 이미지는 사용할 수 없습니다.
필요하다면 로컬로 내려받은 다음 gpt-3.5-turbo 모델에 입력하기 위해 웹에 올린 뒤 해당 url을 query에 기입해줘야 합니다.

## sample
![sample](sample.png)
html sample은 소스코드를 확인해주시기 바랍니다.
