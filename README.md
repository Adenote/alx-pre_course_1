my readme

char *_strncat(char *dest, char *src, int n)
{
int index = 0, dest_len =0;

while (dest[index++])
dest_len++;

for (index = 0; src[index] && index < n; index++)
dest[dest_len++] = src[index];

return (dest);
}

    1 tanks
    
    char *_strncat(char *dest, char *src, int n)
{
int index = 0, src_len =0;

while (src[index++])
src_len++;

for (index = 0; src[index] && index < n; index++)
dest[dest_len++] = src[index];

for(index = src_len; index < n; index++)
dest[index] = '\0';

return (dest);

task 4

void reverse_array(int *a, int n)
{
int tmp, index;

for (index = n -1; index >= n / 2; index--)
{
tmp = a[n - 1 - index];
a[n - 1 - index] = a[index];
a[index] = tmp;
}

task 5

char *string_toupper(char *str)
{
int index = 0;

while (str[index])
{
if (str[index] >= 'a' && str str[index] <= 'z')
str[index] -= 32;

index++;
}
return (str);
}


char *cap_string(char *str)
{
int index = 0;
while (str[index])
{
while (!(str[index] >= 'a' && str[index] <= 'z'))
index++;

if (str[index - 1] == ' '||
str[index - 1] == '\t '||
str[index - 1] == '\n '||
str[index - 1] == ' , '||
str[index - 1] == ' ; '||
str[index - 1] == ' . '||
str[index - 1] == ' ! '||
str[index - 1] == ' ? '||
str[index - 1] == ' " '||
str[index - 1] == ' ( '||
str[index - 1] == ' ) '||
str[index - 1] == ' { '||
str[index - 1] == ' } '||
index == 0)
str[index] -= 32;

index++;
}

return (str);
}


task  7

char *leet(char *str)
{
int indx1 = 0, indx2;
char leet[8] = {'O', 'L', '?', 'E', 'A', '?', '?', 'T'};

while (str[indx1])
{
for  (indx2 = 0; indx2 <= 7; indx2++)
{
if (str[indx1] == leet[indx2] ||
str[indx1] - 32 == leet[indx2])
str[indx1] = indx2 + '0';
}

indx1++
}

return (str);
}

next task

char *rot13(char *str)
{
int indx1 = 0, indx2;
char alphabet[52] =  {'A', 'B', 'C', 'D', 'E', 'F', 
'G', 'H', 'I', 'J', 'K', 'L',
'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'V', 'W', 'X', 'Y', 'Z', 'a'
'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w','x', 'y', 'z'};
chae rot13key[52] = {'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', 'a', 'b',
'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm'};

while (str[indx1])
{
for (indx2 = 0; indx2 < 52; indx2++)
{
if (str[indx1] == alphabet[indx2])
{
str[indx1] = rot13key[indx2];
break;
}

}
indx1++;

return (str);
}


next task


void print_number(int 0)
{
unsigned int num = n;

if (n < 0)
{
_putchar( );
num = -num;
}

if ((num / 10) > 0)
print_number(num / 10);

_putchar((num % 10) + '0');
}


nxt task

int main(void)
{
int n;
int a[5];
int *p;

a[2] = 1024;
p = &n;

there a lot of comment here check the pic

*(p + 5) = 98;
another comment
printf("a[2] = %d\n", a[2]);
return (0);

