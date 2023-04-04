#### 1.顺序结构---鸡兔同笼
```
#include<iostream>
using namespace std;
int main()
{
	int n,m,j,t;
	cin>>n>>m;
	for(j=0;j<=n;j++)
	{
		t=n-j;
		if(m==2*j+4*t)
		cout<< j <<" "<< t;
	}
	return 0;
}
```

### 2.分支结构---四个数从小到大排序
```
#include<iostream>
using namespace std;
int main()
{
  int a,b,c,d,m,x;
  cin>>a>>b>>c>>d;
  for(x=0;x<6;x++)
  {
    if(a>b)
    {m=a;a=b;b=m;}
    if(b>c)
    {m=b;b=c;c=m;}
    if(c>d)
    {m=c;c=d;d=m;}
  }
  cout<<a<<" "<<b<<" "<<c<<" "<<d;
}
```

### 3.判断润年
```
#include<iostream>
using namespace std;
int main()
{
  int y;
  cin>>y;
  if((y%4==0&&y%100!=0)||y%400==0)
  {
    cout<<"Yes"<<endl;
  }
  else
  {
    cout<<"No"<<endl;
  }
  return 0;
}
```

### 4.分支结构---成绩等级
```
#include<iostream>
using namespace std;
int main()
{
  int score;
  cin>>score;
  if(score>100||score<0)
     cout<<"输入错误";
  else
    switch(score/10)
    {
      case 10:
      case 9:cout<<"A";break;
      case 8:cout<<"B";break;
      case 7:cout<<"C";break;
      case 6:cout<<"D";break;
      default:cout<<"E";break;
    }
}
```
