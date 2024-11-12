---
layout: single
title: "[C] shallow copy vs deep copy"
categories: C언어
tag: [C언어, 포인터]
sidebar:
  nav: "docs"
---

# 주소 복사(shallow copy) vs 내용 복사(deep copy)
- 주소를 복사해서 그곳을 찾아가는 방법이 "주소 복사"
- 메모리에 저장된 내용을 복사하는 것이 "내용 복사"
- C언어는 포인터의 주소 값이 변경 될 수 있다는 점이 주의할 점이다.
	- 잘못하면 자신에게 부여된 주소 값을 잃어 버릴 수 있다.
	- 그렇다면 할당된 주소를 모르기 때문에 free 해주지 않으면 오류는 나지 않지만 치명적으로 작동 될 수 있다. -> memory leak(메모리 누수)