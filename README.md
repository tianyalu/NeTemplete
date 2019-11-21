## NeTemplete 函数模板，类模板
### 一、函数模板
1.1 Java中的泛型方法
```java
void T a(T t) {

}
```
1.2 C++中的函数模板
```c
//typename 和 class 效果是一样的
template <typename T>
T a(T i, T j) {
	return i > j ? i : j;
}
int add(int a, int b) {
	return -1;
}
int add(float a, float b) {
	return -1;
}
```
### 二、类模板
```c
template <class T, class E>
class Q {
public:
	T test(T t, E e) {
		return t + e;
	}
};
```
使用
```c
int main()
{
	Q<float, int> q;
	std::cout << q.test(1.1f, 1); //2.1
}
```
