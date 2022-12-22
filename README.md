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
