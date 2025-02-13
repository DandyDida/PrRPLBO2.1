# PrRPLBO2.1

package org.example;

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // Menerima input dari user
        System.out.print("Masukkan nama Anda: ");
        String name = scanner.nextLine();
        System.out.print("Masukkan plat nomer Anda: ");
        String plat = scanner.nextLine();
        
        scanner.close();
        
        // Membuat objek STNK berdasarkan input
        STNK stnk = new STNK(name, plat);

        // Memanggil fungsi printSTNK untuk mencetak informasi STNK
        printSTNK(stnk);
    }

    public static void printSTNK(STNK stnk) {
        System.out.println("Nama\t\t: " + stnk.getPemilik());
        System.out.println("Kode Plat\t: " + stnk.getKodePlat());
        System.out.println("Lokasi\t\t: " + stnk.getLokasi());
    }
}
