# Wave-algorithm
С помощью изменения значений высоты и длины напечатаем волновой узор.
для начала введём целочисленные переменные:

static void pattern(int wave_height,
                        int wave_length)
    {
        int i, j, k, e, n, count, x;
        e = 2;
        x = 1;


Создаём цикл для высоты
for (i = 0; i < wave_height; i++)
        {
            for (j = wave_height; j <= wave_height + i; j++)
                System.out.print(" ");
                
                Создаём цикл для длины
 for (count = 1; count <= wave_length; count++)
            {
        Проверяем промежутки
         
                for (n = (wave_height + wave_height - 2); n >= x; n--)
                    System.out.print(" ");
              
                for (k = 1; k <= e; k++)
                {
                    if (k == 1)
                        System.out.print("/");
                    else if (k == e)
                        System.out.print("\\");
                    else
                        System.out.print(" ");
                }
            }
            Увеличим счётчики на два
            
             x = x + 2;
            e = e + 2;
              
            System.out.println();
        }
    }
    Ввод значений высоты и длины
     public static void main(String args[])
    {
        // изменить значение чтобы уменьшить или увелчить высоту волны
        int wave_height = 4;
  
        // изменить значение чтобы уменьшить или увелчить длину волны
        // 
        int wave_length = 4;
  
        pattern(wave_height, wave_length);
    }
}
