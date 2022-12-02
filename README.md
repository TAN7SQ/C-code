# C-code
just for leaning    


##目的,用三个指针数组加上指针数组的运算,遍历整个
int main()
{
	int arr0[5] = { 1,2,3,4,5 };//identify three arr
	int arr1[5] = { 11,22,33,44,55 };
	int arr2[5] = { 111,222,333,444,555 };
	int* ptoarr[3];
	  ptoarr[0] = arr;//为指针赋值
	  ptoarr[1] = arr1;
	  ptoarr[2] = arr2;
	for (int i = 0; i < 3; i++)
	 {
		int** p = ptoarr + i;//定位指针函数,从
		  for (int j = 0; j < 5; j++)
			   printf("%d ", *(*p + j));
		printf("\n");
	 }
	printf("\n");
}



理解代码,原始数组相当于是一栋楼中的同楼层
