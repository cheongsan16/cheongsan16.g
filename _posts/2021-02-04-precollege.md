---
layout: post
title:  예비대학 - 코딩의 시작 실습
date:   2021-02-04 21:52:55 +0300
image:  /assets/images/blog/post-3.jpg
author: Haeun
tags:   java
---

**페이지 목적**
예비대학이라 하여, 신입생OT 겸? 2월쯤 되면 다들 놀기도 지겨울테니 뭐라도 배우라는 듯 학교에서 강의를 올려줬다.
그 중 코딩의 시작이란 과목이 있어 들어보았다. 교수님께서 너무 열정적으로 강의를 하셔서 무심히 보고만 있기가 힘들었다.
또한, 교수님께서 손수 실습 시범을 보이시며 설명하시는 걸 듣다보면 목소리에 즐거움이 뚝뚝 떨어져 나도 당장 코딩을 하고싶게 만들었다.
그런데! 이 강의에서는 아주 기초적인 것들만 쉽게 가르쳐주시기 위해 스크래치를 사용하시더라..
2년 전, 우리학교에서 했던 (그때는 고등학생으로서 와! 대학에서 캠프한대~ 하고 참여했던..) 캠프에서 간단한 아두이노 실습을 위해 엔트리를 사용한 이후로 한번도 만져본 적 없는 블럭코딩...
프로그래밍을 파이썬으로 시작한 나에게는 오히려 블럭코딩이 귀찮고 어렵다.
그래서! 요새 배우기 시작한 자바로 실습과제를 풀어보기로 했다.
1년 반동안 파이썬을 해와서 파이썬으로 코딩하는데는 꽤 익숙하지만, 자바는 실습경험이 없기 때문에 자바 문법에 익숙해지기 위해 자바를 선택했다.

**첫번째 : BMI지수 구하기**
```
import java.util.Scanner;

public class frist {
	public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("체중을 입력하세요:"); 
        int weight = scanner.nextInt();
        System.out.println("키를 입력하세요:"); 
        int height = scanner.nextInt();
        scanner.close();
        double m_height = (height * 0.01);
        double h = (m_height * m_height);
//        System.out.println(h);
        System.out.println(String.format("%.2f", weight/h));
    }
}
```
Scanner, 산술연산자를 사용한 아주 간단한 코드
(아주 간단한 문제라 할 말이 없네유!)
초반이고 아무것도 모르는 애들 대상이기 때문에, 내가 개발자이면서 사용자일 수 있는 '묻고 기다리기 - 대답'을 많이 쓰는 코드를 굉장히 많이 쓰셨다.
덕분에 import도 하나한 코드가 됨(?)

파이썬이랑 많은 차이가 날 줄 알았는데 전혀... 안녕하십니까 -> 안녕하세요 이 정도 차이밖에 못 느끼겠다
다음은 그리기 문제라 (할 순 있겠지만) 패스

**두번째 : **
빠른 시일 내 찾아옵니다 😜
