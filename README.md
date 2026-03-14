# Program Java: Bangun Ruang, Array 1 Dimensi, dan Array 2 Dimensi

# Deskripsi Program
Lingga chezya poetra (312510169)
Faza fauzan adhima   (312510148)

Program ini dibuat menggunakan bahasa pemrograman Java untuk memenuhi tugas pemrograman dasar.
Program terdiri dari tiga bagian utama yaitu:

1. Program Bangun Ruang untuk menghitung volume kubus dan balok.
2. Program Array 1 Dimensi untuk menyimpan beberapa nilai dalam sebuah array dan menghitung jumlahnya.
3. Program Array 2 Dimensi untuk membuat matriks 3x3 dan menampilkan hasilnya.

---

# 1. Program Bangun Ruang

Code Program

import java.util.Scanner;

public class BangunRuang {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        double sisi, p, l, t;
        double volumeKubus, volumeBalok;

        System.out.println("PROGRAM BANGUN RUANG");

        System.out.print("Masukkan sisi kubus: ");
        sisi = input.nextDouble();

        volumeKubus = sisi * sisi * sisi;

        System.out.println("Volume Kubus = " + volumeKubus);

        System.out.print("\nMasukkan panjang balok: ");
        p = input.nextDouble();

        System.out.print("Masukkan lebar balok: ");
        l = input.nextDouble();

        System.out.print("Masukkan tinggi balok: ");
        t = input.nextDouble();

        volumeBalok = p * l * t;

        System.out.println("Volume Balok = " + volumeBalok);
    }
}

# Penjelasan Code

- "Scanner" digunakan untuk membaca input dari pengguna.
- Program meminta pengguna memasukkan sisi kubus untuk menghitung volume kubus.
- Rumus volume kubus adalah s × s × s.
- Program juga meminta panjang, lebar, dan tinggi untuk menghitung volume balok.
- Rumus volume balok adalah p × l × t.

---

# 2. Program Array 1 Dimensi

Code Program

import java.util.Scanner;

public class Array1Dimensi {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        int[] data = new int[5];
        int jumlah = 0;

        System.out.println("PROGRAM ARRAY 1 DIMENSI");

        for(int i = 0; i < 5; i++){

            System.out.print("Masukkan angka ke-" + i + " : ");
            data[i] = input.nextInt();

            jumlah += data[i];
        }

        System.out.println("\nIsi Array:");

        for(int i = 0; i < 5; i++){

            System.out.print(data[i] + " ");
        }

        System.out.println("\nJumlah semua elemen = " + jumlah);
    }
}

# Penjelasan Code

- Program menggunakan array satu dimensi dengan ukuran 5.
- Pengguna diminta memasukkan 5 angka.
- Nilai yang dimasukkan disimpan ke dalam array.
- Program menampilkan seluruh isi array.
- Program juga menghitung jumlah seluruh elemen array.

---

# 3. Program Array 2 Dimensi

Code Program

import java.util.Scanner;

public class Array2Dimensi {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        int[][] matriks = new int[3][3];
        int jumlah = 0;

        System.out.println("PROGRAM ARRAY 2 DIMENSI");

        for(int i = 0; i < 3; i++){
            for(int j = 0; j < 3; j++){

                System.out.print("Masukkan nilai [" + i + "][" + j + "] : ");
                matriks[i][j] = input.nextInt();

                jumlah += matriks[i][j];
            }
        }

        System.out.println("\nHasil Matriks:");

        for(int i = 0; i < 3; i++){
            for(int j = 0; j < 3; j++){

                System.out.print(matriks[i][j] + " ");
            }
            System.out.println();
        }

        System.out.println("\nJumlah semua elemen matriks = " + jumlah);
    }
}

# Penjelasan Code

- Program menggunakan array dua dimensi (matriks) berukuran 3 × 3.
- Pengguna diminta memasukkan 9 angka.
- Angka disimpan dalam matriks menggunakan indeks "[baris][kolom]".
- Program kemudian menampilkan matriks yang sudah diisi.
- Program juga menghitung jumlah seluruh elemen matriks.

---

# Ringkasan

Program ini menunjukkan penggunaan dasar bahasa pemrograman Java, khususnya dalam:

- Menggunakan input dari pengguna
- Menghitung volume bangun ruang
- Menggunakan array 1 dimensi
- Menggunakan array 2 dimensi (matriks)

Program ini membantu memahami konsep dasar struktur data array dan perulangan (loop) dalam Java.

---

# Dokumentasi Program

Contoh tampilan saat program dijalankan:

"Output Program" (screenshot.png)

(Ganti "screenshot.png" dengan gambar hasil program yang sudah diupload ke repository GitHub.)
