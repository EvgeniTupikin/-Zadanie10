# -Zadanie10
Задание номер 1
public class Main
{
	public static void main(String[] args) {
	
	int[][] a=new int[10][10];
  for (int i=0;i < a.length;i++){
    for (int j=0;j < a[i].length;j++){
      a[i][j]=(int)(Math.random()*10);
      }
     }
for (int i=0;i < a.length;i++,System.out.println("Ответик")){
for (int j=0;j < a[i].length;j++){
System.out.print(a[i][j]+" ");

           }
		}
		}
		}



Задание номер 2
public class Main
{
	
public static void main(String[] args) {
    
        int[][] arr = new int[4][4];
        int max = 0;
        int stroka = 0;
        //аполняем массив может тебе это не понадобится делал для наглядности
        for (int i = 0; i < arr.length; i++) {
            System.out.println(" " + "\n");
            for (int j = 0; j < arr[i].length; j++) {
                arr[i][j] = 0 + (int) (Math.random() * 10);
                System.out.print(arr[i][j] + "    ");
            }
        }
        //ищем максимальное число в диаганале матрицы
 
        for (int i = 0, j = arr.length - 1; i < arr.length && j >= 0; i++, j--) {
            if (arr[i][i] > max && arr[i][i] > arr[j][i]) {
                max = arr[i][i];
                stroka = i;
            } else if (arr[j][i] > max && arr[j][i] > arr[i][i]) {
                max = arr[j][i];
                stroka = j;
            }
        }
        System.out.println("\n" + "Вывожу строку в которой находится максимум" + "\n");
 
        for (int i = 0; i < arr[stroka].length; i++) {
            System.out.print(arr[stroka][i] + "  ");
        }
        System.out.println("\n" + "Вывожу максимальное значение побочной и главной матрицы " + max);
       
    }
 
    
}
	
		
Задание номер 3
public class Main {
 
    public static void main(String[] args) {
               
    int array[][] = new int[3][3];
        int sum = 0;
        //Заполняем массив данными
        for (int i = 0; i < array.length; i++) {
            for (int j = 0; j < array[i].length; j++) {
                array[i][j] = (int) ((Math.random() * 10)+1);   
                System.out.println(array[i][j] + "    ");
            }
        }
        //Считаем все элементы двумерного массива
        for (int i = 0; i < array.length; i++) {
            for (int j = 0; j < array[i].length; j++) {
                sum += array[i][j];
            }
        }
        System.out.println("Сумма всех элементов двумерного массива = "+sum);

    }
}   
