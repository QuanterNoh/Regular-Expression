## 정규 표현식?
정규 표현식은 문자열에서 특정한 규칙을 가진 문자열을 찾거나 조작하는데 사용되는 방법입니다


## 정규 표현식은 주로 어디에서 사용되는가?
정규 표현식은 패턴 매칭, 검색, 추출, 치환 등의 기능을 통해 데이터 전처리, 텍스트 처리, 문자열 검색 및 필터링 등의 작업을 수행할 수 있어 데이터 분석 및 머신러닝 분야에서 유용하게 사용됩니다.


## Python에서 정규 표현식의 기본 사용법
python에서는 re 모듈을 불러와 정규 표현식을 진행할 수 있습니다.

    import re
    
re 모듈에서 주로 사용되는 함수는 다음과 같습니다.
    
    # 정규 표현식을 정규 표현식 객체로 컴파일하여 반환
    re.compile(pattern, flags=0)
    
    # 정규 표현식과 일치하는 문자열을 검색하여, 첫번째로 매칭된 객체 혹은 None을 반환
    re.search(pattern, string, flags=0)
    
    # 문자열의 처음부터 정규 표현식과 일치하는 패턴을 찾아, 매칭된 객체 혹은 None을 반환
    re.match(pattern, string, flags=0)
    
    # 정규 표현식과 일치하는 모든 패턴을 찾아 리스트로 반환
    re.findall(pattern, string, flags=0)
    
    # 정규 표현식과 일치하는 모든 패턴을 다른 문자열로 치환하며 count 값을 조절하여 치환 횟수 조정
    re.sub(pattern, repl, string, count=0, flags=0)
    
    # 정규 표현식에 해당하는 패턴을 기준으로 문자열을 분리하여 리스트로 반환, maxsplit 값을 조절하여 분리 횟수 조정
    re.split(pattern, string, maxsplit=0, flags=0)
