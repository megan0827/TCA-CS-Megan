# 📌 Assignment 4-1

## 1. 제목

ChatGPT를 활용한 자료구조 선택과 최적화

## 2. 이름

최유정(Megan)

## 3. 제출일

24.10.14 (월)

## 4. 과제 목표

> ChatGPT를 활용하여 어떤 자료구조가 더 효율적일지 배우는 것입니다.


## 5. ChatGPT 활용

### 👉 질문 내용

자료구조(리스트, 딕셔너리, 집합 등)를 사용하여 학생들의 이름과 성적을 관리하는 프로그램을 작성해 주세요.

### 👉 ChatGPT 답변 요약

생들의 이름과 성적을 관리할 수 있는 파이썬 프로그램을 작성해보겠습니다. 이 프로그램에서는 리스트와 딕셔너리를 사용하여 학생들의 데이터를 저장하고 관리할 것입니다.

기능:

1. 학생 추가
2. 성적 수정
3. 성적 조회
4. 전체 학생 목록 및 성적 출력
5. 학생 삭제


## 6. 자료구조 선택 이유

리스트와 집합, 딕셔너리를 이용했습니다. 

## 7. 코드 작성 과정

ChatGPT를 이용했습니다. 

## 8. 코드 실행 결과

# 학생 성적 관리 프로그램

# 학생 정보를 저장할 딕셔너리
students = {}

# 학생 추가 함수
def add_student(name, score):
    if name in students:
        print(f"{name} 학생은 이미 존재합니다.")
    else:
        students[name] = score
        print(f"{name} 학생이 추가되었습니다.")

# 성적 수정 함수
def update_score(name, new_score):
    if name in students:
        students[name] = new_score
        print(f"{name} 학생의 성적이 {new_score}로 수정되었습니다.")
    else:
        print(f"{name} 학생을 찾을 수 없습니다.")

# 성적 조회 함수
def get_score(name):
    if name in students:
        print(f"{name} 학생의 성적: {students[name]}")
    else:
        print(f"{name} 학생을 찾을 수 없습니다.")

# 전체 학생 목록 및 성적 출력 함수
def display_students():
    if students:
        print("전체 학생 목록:")
        for name, score in students.items():
            print(f"이름: {name}, 성적: {score}")
    else:
        print("등록된 학생이 없습니다.")

# 학생 삭제 함수
def remove_student(name):
    if name in students:
        del students[name]
        print(f"{name} 학생이 삭제되었습니다.")
    else:
        print(f"{name} 학생을 찾을 수 없습니다.")

# 메인 실행
while True:
    print("\n학생 성적 관리 프로그램")
    print("1. 학생 추가")
    print("2. 성적 수정")
    print("3. 성적 조회")
    print("4. 전체 학생 목록 보기")
    print("5. 학생 삭제")
    print("6. 프로그램 종료")
    
    choice = input("원하는 작업의 번호를 입력하세요: ")
    
    if choice == '1':
        name = input("학생 이름을 입력하세요: ")
        score = float(input("성적을 입력하세요: "))
        add_student(name, score)
    
    elif choice == '2':
        name = input("성적을 수정할 학생 이름을 입력하세요: ")
        new_score = float(input("새로운 성적을 입력하세요: "))
        update_score(name, new_score)
    
    elif choice == '3':
        name = input("성적을 조회할 학생 이름을 입력하세요: ")
        get_score(name)
    
    elif choice == '4':
        display_students()
    
    elif choice == '5':
        name = input("삭제할 학생 이름을 입력하세요: ")
        remove_student(name)
    
    elif choice == '6':
        print("프로그램을 종료합니다.")
        break
    
    else:
        print("잘못된 입력입니다. 다시 시도하세요.")



## 9. 문제 해결 과정 및 배운점

리스트와 딕셔너리, 집합을 이용하여 프로그램을 만드는 법을 배웠습니다. 
