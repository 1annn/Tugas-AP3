# Tugas-AP3


### Sintak Faktorial
    #include <stdio.h>

    int faktorial(int num)
    {
        if (num == 0)
        {
            return 1;
        }
        return num * faktorial(num - 1);
    }

    int main()
    {
        int bil, hasil;
        printf("Masukkan bilangan: ");
        scanf("%d", &bil);
        hasil = faktorial(bil);
        printf("Faktorial dari %d! = %d ", bil, hasil);
        return 0;
    }
    
### Sintak Besar Kecil
    #include <stdio.h>

    int a, b, c, max, min;
    void fungsi_bk()
    {
        if (a > b)
        {
            max = a;
            min = b;
        }
        else
        {
            max = b;
            min = a;
        }
        if (c > max)
            max = c;
        if (c < min)
            min = c;
    }

    void main()
    {
        printf("Masukan bilangan 1 : ");
        scanf("%d", &a);
        printf("Masukan bilangan 2 : ");
        scanf("%d", &b);
        printf("Masukan bilangan 3 : ");
        scanf("%d", &c);
        fungsi_bk();
        printf("\nBilangan terbesar : %d\n", max);
        printf("Bilangan terkecil : %d", min);
    }
