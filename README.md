# PTA_7-8
# 超速判断
# 模拟交通警察的雷达测速仪。输入汽车速度，如果速度超出60 mph，则显示“Speeding”，否则显示“OK”。

# 输入格式：输入在一行中给出1个不超过500的非负整数，即雷达测到的车速。

# 输出格式：在一行中输出测速仪显示结果，格式为：Speed: V - S，其中V是车速，S或者是Speeding、或者是OK。
```cpp
#include<iostream>

using namespace std;
int main() {
	int speed;
	cin >> speed;
	if (speed <0 ||speed>500) {
		cout << "Invalid speed" << endl;
			return 0;
	}

	if (speed > 60 ) {
		cout <<"Speed: " << speed << " - " << "Speeding" << endl;  //需为英文半角:
	}
	else {
		cout <<"Speed: " << speed << " - " << "OK" << endl;
	}
	
	return 0;
}