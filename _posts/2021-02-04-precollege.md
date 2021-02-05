---
layout: post
title:  예비대학 - 코딩의 시작 실습
date:   2021-02-04 21:52:55 +0300
image:  /assets/images/blog/post-3.jpg
author: Haeun
tags:   java
---

**코딩의 시작 듣는 블로그**

예비대학이라 하여, 신입생OT 겸? 2월쯤 되면 다들 놀기도 지겨울테니 뭐라도 배우라는 듯 학교에서 강의를 올려줬다. 
등록금 내는만큼 어떻게는 뽑아먹으려면 주는 거 다 이용해야 안되겠나, 싶어 코딩의 시작이란 과목부터 들어보았다.
<br>그런데 교수님께서 너무 열정적으로 강의를 하셔서 무심히 보고만 있기가 힘들었다. 교수님께서 손수 실습 시범을 보이시며 설명하시는 걸 듣다보면 목소리에 즐거움이 뚝뚝 떨어져 나도 당장 코딩하고 싶어질 정도였다.<br>
흥미를 갖고 듣던 중, 예상했던 난관(?)에 봉착했다. 이 강의에서는 아주 기초적인 것들만 쉽게 가르쳐주시기 위해 스크래치를 사용하시더라..
2년 전, 우리학교에서 했던 (그때는 고등학생으로서 와! 어쩌구대학에서 캠프한대~ 하고 참여했던..) 캠프에서 간단한 아두이노 실습을 위해 엔트리를 사용한 이후로 한번도 만져본 적 없는 블럭코딩...<br>
프로그래밍을 파이썬으로 시작한 나에게는 오히려 블럭코딩이 귀찮고 어렵기 때문에, 요새 배우기 시작한 자바로 실습과제를 풀어보기로 했다. (절대 그냥 들을 순 없어..)

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
        System.out.println(String.format("%.2f", weight/h));
    }
}
```
Scanner, 산술연산자를 사용한 아주 간단한 코드
(아주 간단한 문제라 할 말이 없네유!)<br>
초반이고 아무것도 모르는 학생 대상이기 때문에, 내가 개발자이면서 사용자일 수 있는 '묻고 기다리기 - 대답'을 블럭을 굉장히 많이 쓰셨다.
덕분에 import가 하나 필요한 코드가 됨(?)

파이썬이랑 많은 차이가 날 줄 알았는데 전혀... 안녕하십니까 -> 안녕하세요 이 정도 차이밖에 못 느끼겠다.<br>
다음은 그리기 문제라 (할 순 있겠지만) 패스

**두번째 : 구구단 출력하기**<br>
(사실 앞에 한 강의 더 있었지만... for문 하나면 끝나는 것들 뿐이라 건너뜀)<br>
스타일에 따라 두 가지 형태로 만들었다.<br>

1. java.util.Arrays 클래스 사용
```
import java.util.Arrays;

public class second {
	public static void main(String[] args) {
		for (int a = 2; a<10; a++){
			int[] table = new int[9];
			for (int b = 1; b<10; b++){
				table[b-1] = a * b;
			}
			System.out.println(a + "단 : " + Arrays.toString(table));
		}
	}
}
```

배열 검색하는 중 java.util.Arrays 클래스를 발견했고, 바로 사용해보았다.<br>
```
2단 : [2, 4, 6, 8, 10, 12, 14, 16, 18]
3단 : [3, 6, 9, 12, 15, 18, 21, 24, 27]
4단 : [4, 8, 12, 16, 20, 24, 28, 32, 36]
5단 : [5, 10, 15, 20, 25, 30, 35, 40, 45]
6단 : [6, 12, 18, 24, 30, 36, 42, 48, 54]
7단 : [7, 14, 21, 28, 35, 42, 49, 56, 63]
8단 : [8, 16, 24, 32, 40, 48, 56, 64, 72]
9단 : [9, 18, 27, 36, 45, 54, 63, 72, 81]
```


