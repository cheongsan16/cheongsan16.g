---
layout: post
title:  linked list 구현
date:   2021-05-01 01:40:29 +0300
image:  /assets/images/blog/post-2.jpg
author: Haeun
tags:   java
---

**서론**

Linkedlist를 JAVA로 구현한 코드 설명<br>
우선, Linkedlist, 연결리스트는 각 노드가 데이터와 포인터를 가지고 일렬로 연결된 방식으로 데이터를 저장하는 자료구조이다.<br>
연결리스트는 연결되 노드 사이에 새로운 노드를 추가하거나, 기존 노드를 삭제할 수 있다는 특징을 가진다.<br>
텐션이 낮은 상태라 별 말없이 바로 본론으로..

**노드 생성**

노드를 생성한다. 

```
public class Node {
	public int data; //데이터
	public Node next; //포인터

	public Node(int data) { //생성자 - 
		this.data = data;
	}

	public void print() {
		System.out.print("{" + data + "}");
	}
}
```
