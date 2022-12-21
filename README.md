# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		      : Shafa Dea Secaria
<br>NIM		        :	1227050124
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Matriks adalah susunan bilangan-bilangan berbentuk persegi panjang yang diatur dalam baris atau kolom dengan dibatasi kurung. Bilangan yang tersusun dalam matriks disebut elemen/unsur matriks. Baris adalah susunan bilangan-bilangan yang mendatar (horizontal), sedangkan kolom adalah susunan bilangan-bilangan yang tegak (vertikal). Ordo matriks adalah banyaknya elemen baris dan banyaknya elemen kolom dari suatu matriks. Jika sebuah matriks memiliki i baris dan j kolom, maka matriks tersebut berordo i x j, dapat dituliskan Ai.j. Pemanfaatan matriks antara lain pada bidang keamanan komputer serta untuk pemrograman yang membutuhkan array dalam Ilmu Komputer.

## Source Code
#include <iostream>
using namespace std;

int main() {
	
	cout << "=====================================\n";
	cout << "UAS DASAR PEMROGRAMAN \n";
	cout << "PROGRAM ARRAY 2 DIMENSI     \n\n";
	cout << "Nama  : Shafa Dea Secaria" << endl;
	cout << "NIM   : 1227050124" << endl;
	cout << "Kelas : Informatika-C " << endl;
	cout << "=====================================\n\n";
	
	cout<< "=============================================================================\n";
	cout<< "1. Menginput Banyaknya Baris dan Kolom. Kemudian Baris dan Kolomnya Ditukar\n\n";
	
 	int A [100] [100];
	int baris, kolom, b, k;
	
	cout << "Masukkan Jumlah Baris Matriks: ";
	cin >> baris;
	cout << "Masukkan Jumlah Kolom Matriks: ";
	cin >> kolom;
	cout << endl;
	
	for (b = 0; b < baris; b++) {
		for (k = 0; k< kolom; k++) {
			  cout << "Baris " << b << ", Kolom " << k << " = ";
			  cin >> A [b][k];
		}
		cout << endl;
	}
	cout << "Matriks Sebelum Diubah"<<endl;
	for (b = 0; b < baris; b++){
		for (k = 0; k < kolom; k++){
			 cout << A [b][k] << " ";
		}
		cout << endl;
	}
	cout << "\nHasil Transpose Matriks" << endl;
	for (b = 0; b < kolom; b++){
		for (k = 0; k < baris; k++){
			 cout << A[k][b] << " ";
		}
		cout << endl;
	}
	cout << "=============================================================================\n\n";
	
	
	cout << "===================================================\n";
	cout << "2. Menampilkan Bilangan Yang Habis Dibagi 3, 5, 7.\n\n";	
	
	cout << "Masukkan Jumlah Baris Matriks : ";
	cin >> baris;
	cout << "Masukkan Jumlah Kolom Matriks : ";
	cin >> kolom;
	cout << endl;
	
	for (b = 0; b < baris; b++){
		for (k = 0; k < kolom; k++){
			  cout << "Baris " << b << ", Kolom " << k << " = ";
			  cin >> A [b][k];
		}
		cout << endl;
	}
	
	cout << "Matriks" << endl ;
	for (b = 0; b < baris; b++){
		for (k = 0; k < kolom; k++) {
			 cout << A [b][k] << " ";
		}
		cout << endl;
	}
	cout << endl << "Nilai Matriks yang Habis Dibagi 3,5,7 \n";
	for (b = 0; b < baris; b++){
		for (k = 0; k < kolom; k++){
			if(A [b][k] %3 == 0){
				cout << "     " << A [b][k];
			}
			else if(A [b][k] %5 == 0){
				cout<<"     " << A [b][k];
			}
			else if(A [b][k] %7 == 0){
				cout << "     " << A [b][k];
			}
			else {
				cout << "     " << endl;
			}
		}
		cout<<endl;
	}
		cout << "===================================================\n";
	
	return 0;
}

## Output
### =====================================
UAS DASAR PEMROGRAMAN
PROGRAM ARRAY 2 DIMENSI

Nama  : Shafa Dea Secaria
NIM   : 1227050124
Kelas : Informatika-C
=====================================

=============================================================================
1. Menginput Banyaknya Baris dan Kolom. Kemudian Baris dan Kolomnya Ditukar

Masukkan Jumlah Baris Matriks: 2
Masukkan Jumlah Kolom Matriks: 3

Baris 0, Kolom 0 = 1
Baris 0, Kolom 1 = 2
Baris 0, Kolom 2 = 3

Baris 1, Kolom 0 = 4
Baris 1, Kolom 1 = 5
Baris 1, Kolom 2 = 6

Matriks Sebelum Diubah
1 2 3
4 5 6

Hasil Transpose Matriks
1 4
2 5
3 6
=============================================================================

===================================================
2. Menampilkan Bilangan Yang Habis Dibagi 3, 5, 7.

Masukkan Jumlah Baris Matriks : 3
Masukkan Jumlah Kolom Matriks : 2

Baris 0, Kolom 0 = 7
Baris 0, Kolom 1 = 8

Baris 1, Kolom 0 = 9
Baris 1, Kolom 1 = 3

Baris 2, Kolom 0 = 5
Baris 2, Kolom 1 = 6

Matriks
7 8
9 3
5 6

Nilai Matriks yang Habis Dibagi 3,5,7
     7
     
     9     3
     
     5     6
===================================================
