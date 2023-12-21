#include <iostream>
#include <sys/time.h>
#include <cstdlib>
#include <string.h>
using namespace std;
// Запускать программу так: matrix.exe <n>
// Где n - размерность матриц для перемножения
 // Рекомендуется брать n где-то около 500-1000
int main(int argc, char **argv) {
// Говорим пользователю, что программа стартовала cout << "Started....";
// Делаем отметку о начале выполнения программы struct timeval curr_time{};
 gettimeofday(&curr_time, nullptr);
time_t start_time = (curr_time.tv_sec * 1000) + (curr_time.tv_usec / 1000);
// Получаем размерность матриц из консоли или используем дефолтную

 int n = 100;
if (argc == 2) {
    n = atoi(argv[1]);
}
// Инициализируем модуль рандома с определённым начальным значением
// Это позволит генерировать одинаковые массивы при каждом запуске
srand(1);
// Инициализируем первый и второй массивы со случайными числами
int **arr1 = new int*[n];
 int **arr2 = new int*[n];
long **rez = new long*[n];
for (int i=0; i<n; i++) {
    arr1[i] = new int[n];
    arr2[i] = new int[n];
    rez[i] = new long[n];
}
for (int i=0; i<n; i++) { for (int j=0; j<n; j++) {
        arr1[i][j] = rand();
        arr2[i][j] = rand();
    }
}
// Перемножаем массивы
 for (int i=0; i<n; i++) { for (int j=0; j<n; j++) {
} }
rez[i][j] = 0;
for (int k=0; k<n; k++) {
    rez[i][j] += arr1[i][k] * arr2[k][j];
}
// Делаем отметку о завершении выполнения программы
gettimeofday(&curr_time, nullptr);
time_t end_time = (curr_time.tv_sec * 1000) + (curr_time.tv_usec / 1000);
 cout << "Execution time: " << (end_time - start_time) << " ms" << endl;
// Освобождаем память
for (int i=0; i<n; i++) {
    delete [] arr1[i];
     delete [] arr2[i];
    delete [] rez[i];
}
delete [] arr1;
delete [] arr2;

     delete [] rez;
return 0; }
