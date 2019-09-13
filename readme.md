# uml序列图

## 快速开始

1. 向A发送一条消息

```
A.method()
```

2. 向B发送一条消息

```
A.method() {
	B.method()
}
```

3. 创建一个对象C

```
A.method() {
	B.method()
	new C()
}
```

4. 条件判断

```
A.method() {
	B.method()
	new C()
	if(condition) {
		C.doSomething()
	} else {
		C.doSomethingElse()
	}
}
```

5. 条件循环

```
while(true) {
	C.repeat()
}
```
![zenuml1]("/images/zenuml1.png")

## example

> restful服务

```
response = BookControleer.getBook(id) {
	book = BookService.getById(id) {
		book = BookRepository.findChild(id)
	}
	response = createResponse(book)
}
```
![zenuml2]("/images/zenmul1.png")

## zenuml地址

![https://app.zenuml]https://app.zenuml.com/