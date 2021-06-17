# hello-word
一段简单的入门代码！
// 第一个项目.cpp : 此文件包含 "main" 函数。程序执行将在此处开始并结束。
//

#include<iostream>
#include<math.h>
using namespace std;
double juli(double x1, double y1,
	double x2 = 0, double y2 = 0)
	//计算双精度坐标1（x1,y1）与坐标2（x2,y2）间距
{
	double n;
	n = sqrt((x1 - x2) * (x1 - x2) + (y1 - y2) * (y1 - y2));
	return n;
}
int juli(int x1, int  y1, int x2 = 0, int y2 = 0)
//计算整型坐标1（x1,y1）与坐标2（x2,y2）间距
{
	int m;
	m = sqrt((x1 - x2) * (x1 - x2) + (y1 - y2) * (y1 - y2));
	return m;
}
int main()
{
	cout << "请输入(x1,y1),(x2,y2)" << endl;
	int x1, y1, x2, y2;
	double a1, b1, a2, b2;
	cin >> x1 >> y1 >> x2 >> y2;
	cin >> a1 >> b1 >> a2 >> b2;
	int m;
	m = juli(x1, y1, x2, y2);
	cout << "距离为" << m << endl;
	double  n;
	n = juli(a1, b1, a2, b2);
	cout << "距离为" << n << endl;
	return 0;
}


// 运行程序: Ctrl + F5 或调试 >“开始执行(不调试)”菜单
// 调试程序: F5 或调试 >“开始调试”菜单

// 入门使用技巧: 
//   1. 使用解决方案资源管理器窗口添加/管理文件
//   2. 使用团队资源管理器窗口连接到源代码管理
//   3. 使用输出窗口查看生成输出和其他消息
//   4. 使用错误列表窗口查看错误
//   5. 转到“项目”>“添加新项”以创建新的代码文件，或转到“项目”>“添加现有项”以将现有代码文件添加到项目
//   6. 将来，若要再次打开此项目，请转到“文件”>“打开”>“项目”并选择 .sln 文件
