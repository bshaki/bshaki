#include <stdio.h>
#define YES 1 
#define NO 0 
#define N 2
 
int lr1(void)
{
    float bb = 1, aa = 1, a = 1, b = 0.2, c = -0.35;
    float sum = -0.2;
    float mul = -0.35;
    scanf("a = %f, b = %f,c = %f", &a, &b, &c);
    float i = 0;
    while(i <= 10)
        {
            if(sum - i == mul / i){
                printf("x1 = %f, x2 =%f", sum - i, i);
                return 0;
            } else {
                i = i + 0.1;
            }
        }
       
}
int lr2(void)
{
    int x, N;
    double sum = 0;
    double p = 1;
    printf("enter x and N\n");
    scanf("%d %d", &x, &N);
    for(int i = 1; i <= N; i++){
        p *= x;
        if((i + 1) % 2 == 0){
            sum += (-1) * (p / i) ;
        } else {
            sum += (p / i) ;
        }
    }
    printf("%f", sum);
    return 0;
}

int lr3(void)
{ 
    int cnt, c, prev_c, flag;    
    cnt=0;     
    flag=NO; 
    printf ("самое длинное слово – палиндром \n");    
    while((c = getchar ()) != EOF) 
    { 
        if ((c == ' ') || (c == '.') || (c == '\n') || (c == ',')) 
        {             
            flag=NO;             
            prev_c ==' '; 
        }         
        else 
        { 
            if (flag==NO) 
            {                
                flag=YES;                 
                prev_c=c; 
            }            
            else             {                
                if (prev_c==c) 
                {                     
                    cnt++;                     
                    prev_c=' '; 
                }                 
                else 
                    prev_c=' '; 
            } 
        } 
    } 
    printf("number of words = %d\n", cnt ); 
    return 0;
}

  void reverse_word(char *start, char *end) 
{
    while (start < end) 
       
        *start = *end;
     
        start++;
        end--;
    }
}

void reverse_words(char *input_string) {
    char *start = input_string;
    char *end = input_string;

    while (*end != '\0') {
        if (*end == ' ') {
       reverse_words(start, end - 1);
            start = end + 1;
        }
        end++;
    }

    reverse_words(start, end - 1);
    reverse_words(input_string, end - 1);
}


int lr4(void)
{


    char c;
    int prev_c;
    int flag = YES;

 
    int i = 0;
    {
    while ((c = getchar()) != EOF && i < Maxline - 1) 
        if (c == ' ' || c == '\n') {
            flag = Yes;
        } else {
            flag = No;
        }

        input_string[i] = c;
        i++;
    }
    input_string[i] = '\0';

    reverse_words(input_string);
    printf("%s\n", input_string);

    return 0;
    
}
int lr5(void)


{

    if (min_sum_index != -1) {
        for (int j = (min_sum_index - N < 0 ? 0 : min_sum_index - N); j < (min_sum_index + N + 1 > size ? size : min_sum_index + N + 1); j++) {
            arr[j] = 0;
        }
    }
}

 {
    int arr[] = {3, 1, 4, 2, 8, 5, 7, 6, 9, 10};
    int size = sizeof(arr) / sizeof(arr[0]);
    
  
    
    for (int i = 0; i < size; i++) {
        printf("%d ", arr[i]);
    }
    
    return 0;
    
}
int lr6(void)

{
    int arr[N][K] = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}, {10, 11, 12}};
    float avg[N];
    
    // Print the sorted array
    for (int i = 0; i < N; i++)
    {
        for (int j = 0; j < K; j++)
        {
            printf("%d ", arr[i][j]);
        }
        printf("\n");
    }
    
    return 0;
}
int lr7(void)

int main() 
{
 
 printf("целое число N: ");
 scanf("%lld", &N);
 while (N > 1) {
  bitposition++;
  N >>= 1;
 }
 
 N <<= bitposition;
 
 printf("N обнулить разряды, стоящие правее старшей единицы : %lld", N);
 
 return 0;
}
