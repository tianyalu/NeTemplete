## NeTemplete ����ģ�壬��ģ��
### һ������ģ��
1.1 Java�еķ��ͷ���
```java
void T a(T t) {

}
```
1.2 C++�еĺ���ģ��
```c
//typename �� class Ч����һ����
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
### ������ģ��
```c
template <class T, class E>
class Q {
public:
	T test(T t, E e) {
		return t + e;
	}
};
```
ʹ��
```c
int main()
{
	Q<float, int> q;
	std::cout << q.test(1.1f, 1); //2.1
}
```
