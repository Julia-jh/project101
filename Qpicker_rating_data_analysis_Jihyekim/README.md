- Purpose
    - Find out significant statistical data using Qpicker user's raiting result in both Playstore and Applestore.

- Hypothesis
    1. remove the most frequent rating level, the result would be the ?
    2. remove the least frequent rating level, the result would be the ?

- Step
    1. Scrapping rating data from both Playstore and Applestore.
    2. Calculating statistical data using each of the source and the both.
    3. Checking the both hypothesis
    4. Setting the new agenda or theory.
    

- Library
    - os
    - sys
    - pandas
    - numpy
    - matplotlib.pyplot
    - seaborn
    - time
    - selenium


- reference
    - https://signing.tistory.com/44
        - https://sites.google.com/chromium.org/driver/?pli=1
        - https://www.browserstack.com/guide/difference-between-selenium-remotewebdriver-and-webdriver
    - https://signing.tistory.com/46
        - https://sualchi.tistory.com/13721870
    - https://signing.tistory.com/47
        - https://wikidocs.net/177133
        - https://heytech.tistory.com/293
        - https://western-sky.tistory.com/51
        - https://velog.io/@hwang-eunji/python-%EC%9B%B9-%ED%81%AC%EB%A1%A4%EB%A7%81-feat.-selenium-2-%EC%8B%A4%EC%8A%B5
    - https://www.kaggle.com/datasets/lava18/google-play-store-apps
    
    - https://greeksharifa.github.io/references/2020/10/30/python-selenium-usage/
    - https://liveyourit.tistory.com/17
    - https://dejavuhyo.github.io/posts/patterns-for-writing-better-git-commit-messages/
    
    
    
    
*****************************************************************************************************************

- Issue
    -230427
        1. 도움을 주셔서 감사합니다. 김규백

    - 23426
        1. Ver.2에서 구현하고 싶은 부분 정리해서 나아가 어플 리뷰 스크래이핑하는 코드 표준화 작업 구상 필요
        2. 전체 별점을 사용할 때와, 특정 별점을 제외한 값일 때의 별점 중 어떤 것이 더 유의미한 결과일까?


    - 230425
        1. 데이터를 읽어올 때 빈 값일 경우 조건을 주지 않아 데이터가 전부 연결되지 않음
        > ver2에서 바꾸기
        2. 데이터를 더 읽어와야 할 때, 키보드 입력키인 pagedown을 이용해 화면을 내렸는데, 더 좋은 방법이 없는지 고민중
        > ver2에서 바꾸기
        3. 읽어온 데이터에서 필요없는 부분 잘라내고 데이터타입 바꿔야함
        > .drop() 함수 사용하여 필요없는 행 잘라내고, .astype() 함수 사용하여 열 데이터타입을 object에서 int로 바꿈
    
    - 230424
        1. aria-label 태그 데이터 불러오지 못함
        > .get_attribute('aria-label') 이용
    
    - 230423
        1. driver.find_element를 CLASS_NAME 이용해서 여러 개 불러오는 것 실패함. 단, XPATH는 가능했음
        > driver.find_elements <- s 를 넣어야 함!
        
    - 230422
        1. selenium 라이브러리를 처음 써봄
        > reference 에 관련 블로그를 적어두고, 추후에 사용한 정보를 곁들여 정리
        
        
        
        
        
        
        
        
        
        