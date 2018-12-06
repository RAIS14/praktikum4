# praktikum4

**latihan1.cpp : cara menghitung total pembayaran barang**
````
- mendeklarasikan variable (int) kode,N,jumlah, banyakbarang dan hargabarang
- memasukan jumlah bilangan (banyak barang) yang di inginkan
- membuat perulangan demgan menggunakan for loop "for(jumlah=1;jumlah<=banyak;jumlah++)"
- memasukan bilangan ke dalam variable input (jumlah barang) dengan nilai tertentu
- memasukan bilangan ke dalam variable input (harga satuan) dengan nilai tertentu
- mencetak harga barang (jumlah barang "x" dikali harga satuan "n")
- mencetak total pembayaran (sebelum mendapatkan diskon)
- membuat potongan harga dengan menggunakan if statment (total>1000000 diskon 10%, total>501000 diskon 5%, selain itu tidak dapat diskon)
- memcetak total pembayaran (dengan diskon tertentu)
````
berikut programnya:
````
#include <iostream>

using namespace std;

int main()
{
char pembelian;
int kode, N, jumlah, banyak;
long int total,diskon,akhir, bayar, harga,duit,kembalian;
atas:
cout<<"""""TOKO ALAT MEMANCING RAIS""""""\n";
cout<<"\n";
cout<<"       HARGA BERSAING, KUALITAS NOMOR SATU\n";
cout<<"\n";
cout<<" ""DAFTAR BARANG""\n";
cout<<" 1. KAIL\n";
cout<<" 2. SENAR PANCING\n";
cout<<" 3. KOTAK PANCING\n";
cout<<" 4. TIMAH\n";
cout<<" 5. PELAMPUNG\n";
cout<<" 6. UMPAN IKAN\n";
cout<<" 7. JARING\n";
cout<<"""""""TOKO ALAT MEMANCING RAIS""""""\n";
cout<<"\n";
cout<<"Jumlah Barang Yang Dipesan = ";
cin>>banyak;
jumlah=1;
bayar=0;
for(jumlah=1;jumlah<=banyak;jumlah++)
{ulang:
 cout<<" \n\nMasukan Kode Barang = ";
cin>>kode;
cout<<"\n";
    if (kode==1)
{
    cout<<" Nama Barang     = KAIL\n";
    cout<<" Harga           = Rp. 20000,-\n";
    cout<<" Jumlah Barang   = ";
    cin>>N;
    harga=20000;
    total=harga*N;
    cout<<" Total Harga  = Rp"<<total;
    cout<<"\n";
}
else
    if (kode==2)
{
    cout<<" Nama Barang     = SENAR PANCING\n";
    cout<<" Harga           = Rp. 50000,-\n";
    cout<<" Jumlah Barang   = ";
    cin>>N;
    harga=50000;
    total=harga*N;
    cout<<" Total Harga  = Rp"<<total;
    cout<<"\n";
}
else
    if (kode==3)
{
    cout<<" Nama Barang     = KOTAK PANCING\n";
    cout<<" Harga           = Rp. 50000,-\n";
    cout<<" Jumlah Barang   = ";
    cin>>N;
    harga=50000;
    total=harga*N;
    cout<<" Total Harga  = Rp"<<total;
    cout<<"\n";
}
else
    if (kode==4)
{
    cout<<" Nama Barang      = TIMAH\n";
    cout<<" Harga            = Rp. 2500,-\n";
    cout<<" Jumlah Barang    = ";
    cin>>N;
    harga=2500;
    total=harga*N;
    cout<<" Total Harga  = Rp"<<total;
    cout<<"\n";
}
else
    if (kode==5)
{
    cout<<" Nama Barang     = PELAMPUNG\n";
    cout<<" Harga           = Rp. 5000,-\n";
    cout<<" Jumlah Barang   = ";
    cin>>N;
    harga=5000;
    total=harga*N;
    cout<<" Total Harga  = Rp"<<total;
    cout<<"\n";
}
else
    if (kode==6)
{
    cout<<" Nama Barang     = UMPAN IKAN\n";
    cout<<" Harga           = Rp. 35000,-\n";
    cout<<" Jumlah Barang   = ";
    cin>>N;
    harga=35000;
    total=harga*N;
    cout<<" Total Harga  = Rp"<<total;
    cout<<"\n";
}
else
    if (kode==7)
{
    cout<<" Nama Barang     = JARING\n";
    cout<<" Harga           = Rp. 50000,-\n";
    cout<<" Jumlah Baran    = ";
    cin>>N;
    harga=50000;
    total=harga*N;
    cout<<" Total Harga  = Rp"<<total;
    cout<<"\n";
}
else
{
    cout<<"-Invalid Number-\a";
goto ulang;
}
bayar=bayar+total;
}
    cout<<"\nTotal Bayar\t\t        = Rp"<<bayar<<",-";
    cout<<"\n\n\Masukan Pembayaran  = Rp";cin>>duit;
if((bayar>1000000)){
diskon = bayar*0.10;
cout<<"\nKamu Dapat Diskon 10%\t";
}else
    if((bayar>=501000)&& (bayar<=1000000)){
diskon = bayar*0.05;
cout<<"\nKamu Dapat Diskon 5%\t";
}else
    if((bayar<501000)){
diskon = 0;
cout<<"\nKamu Dapat Diskon 0%\t";
}
else {
diskon = 0;
}
akhir       =bayar-diskon;
kembalian   =duit-akhir;

cout<<"\nKamu Dapat Diskon\t  = Rp"<<diskon<<",-";
cout<<"\nCash Back\t          = Rp"<<kembalian<<",-";
cout<<"\n\n\t\t\t((((THANK YOU))))";
cout<<"\n\n\n\n\nPembelian Baru [y/t] ";cin>>pembelian;
if (pembelian=='y'||pembelian=='Y')
goto atas;
else
cout<<"\n\n\t\t\tProgram Logging Off....";
}

````
**hasil nya** :
![img]https://raw.githubusercontent.com/RAIS14/praktikum4/master/Screenshot_lat1.png

**flowchartnya** :
![img]https://raw.githubusercontent.com/RAIS14/praktikum4/master/flowchart_lat1.jpg