// dibuat oleh fikri nrf SI 04


#include <iostream>
#include <string>
#include <conio.h>
#include <stdio.h>

using namespace std;

struct gunung
{
    int tinggiGn;
    string namaGn;
    string namaProv;

};

int main()
{
    gunung gunungIND;
    char y_t;

    cout << "SELAMAT DATANG DI PROGRAM DATA GUNUNG 34 PROVINSI INDONESIA" << endl;
    cout << "============================================================" << endl;

    cout << endl;
    lagi:
    cout << "Masukan Nama Provinsi untuk mengetahui data Gunung : ";
    cin >> gunungIND.namaProv;

    if(gunungIND.namaProv == "jabar" || gunungIND.namaProv == "Jabar"){
        gunungIND.tinggiGn = 3078;
        gunungIND.namaGn = "Ciremai";
        gunungIND.namaProv = "Jawa Barat";

        cout << "Nama Gunung : " << gunungIND.namaGn << endl;
        cout << "Tinggi Gunung : " << gunungIND.tinggiGn << endl;
        cout << "Berada di Provinsi : " << gunungIND.namaProv << endl;

    }else if(gunungIND.namaProv == "jateng" || gunungIND.namaProv == "Jateng"){
                gunungIND.tinggiGn = 3432;
                gunungIND.namaGn = "Slamet";
                gunungIND.namaProv = "Jawa tengah";

                cout << "Nama Gunung : " << gunungIND.namaGn << endl;
                cout << "Tinggi Gunung : " << gunungIND.tinggiGn << endl;
                cout << "Berada di Provinsi : " << gunungIND.namaProv << endl;

    }else if(gunungIND.namaProv == "jatim" || gunungIND.namaProv == "Jatim"){
                gunungIND.tinggiGn = 3676;
                gunungIND.namaGn = "Semeru";
                gunungIND.namaProv = "Jawa Timur";

                cout << "Nama Gunung : " << gunungIND.namaGn << endl;
                cout << "Tinggi Gunung : " << gunungIND.tinggiGn << endl;
                cout << "Berada di Provinsi : " << gunungIND.namaProv << endl;

    }else{
        cout << "Anda salah memasukan nama provinsi :D" << endl;
    }



    lagi2 :
     cout << "Apakah anda ingin Mengulanginya lagi? (y/t) : ";
     cin >> y_t;

     if(y_t == 'Y' || y_t == 'y')
     {
        goto lagi;
     }else if(y_t == 'T' || y_t == 't'){
                goto selesai;
     }else{
        cout << "Anda salah memasukan karakter!!!!!!!!!!!!!!!!" << endl;
        goto lagi2;
     }

     selesai:
     cout << "Terimakasih Telah mengunjungi program sederhana ini : D" << endl;
    return 0;
}
