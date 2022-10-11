# 10
二分查找_作业


//100带9的数字
int main()
{
	int i = 0;
	int count = 0;
	for (i = 1; i <= 100; i++)
	{
		if (i % 10 == 9)
			count++;
		 if (i / 10 == 9)
			count++;
	}
	//9,19,28...99---10
	//90,91,92...99---10
	printf("count=%d\n", count);
	return 0;
}



//分数求和1/1-1/2+1/3-1/4+...1/99-1/100;
int main()
{
	int i = 0;
	double sum = 0.0;
	int flag = 1;//定义一个变量
	for (i = 1; i <= 100; i++)
	{
		sum += flag * 1.0 / i
			; flag = -flag;
	}
	printf("%lf\n", sum);
	return 0;
}


//求十个数中最大值
int main()
{
	int arr[] = { 5,6,7,8,9,10,11,12,13,14,15 };//改成其它数一样_OK
	int max = arr[0];
	int i = 0;
	int sz = sizeof(arr) / sizeof(arr[0]);
	for (i = 1; i < sz; i++)
	{
		if (arr[i] > max)
		{
			max = arr[i];
		}
	}
	printf("max=%d\n", max);
	return 0;
}



//在屏幕上输出9*9乘法口诀表
int main()
{
	int i = 0;//确定打印9行
		for (i = 1; i <= 9; i++)
		{
			//每进来一次打印一行
			int j = 1;
				for (j = 1; j <= i; j++)
				{
					printf("%d*%d=%-2d ", i, j, i * j);//在%和d之间加上-2表示打印两位，及左对齐
				}
				printf("\n");
		}
	return 0;
}
