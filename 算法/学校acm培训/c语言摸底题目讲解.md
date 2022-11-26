## 数据库操作

```cpp
#include<stdio.h>

char s[5],s1[5],s2[5];
int main(){
	scanf("%s%s%s",&s,&s1,&s2);
	int num=(s[0]=='r')+(s1[0]=='r')+(s2[0]=='r');
	if(num>1){
		puts("NO");
	}else{
		puts("Yes");
		if((s[0]=='r'))puts("u1");
		else if(s1[0]=='r')puts("u2");
		else puts("u3")
	}
	return 0;
} 
```
