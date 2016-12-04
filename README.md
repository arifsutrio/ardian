# ardian
/*——————————————————————————————*/
/* Tugas C++ Membuat Program MENU MAKANAN   */
/*——————————————————————————————*/

#include <conio.h>
#include <iostream.h>
main()
{
char menu,nama_menu[20],bns,beli,lagi, yt;
float totbay,jumbel,totbel,potongan,harga;
kembali:
clrscr();
cout<<""<<endl;
cout<<" Masukkan Kode Makanan [1..3]  : ";cin>>menu;
cout<<" Jumlah Pembelian Pesanan Anda : ";cin>>jumbel;
clrscr();
cout<<"\n ";
cout<<"\t ***BEST FOOD*** \n";
cout<<"\t    BSD  No.20 \n";
cout<<" -------------------------------------------";
cout<<""<<endl;
cout<<" Nama Menu Yang Anda Pesan     :"<<nama_menu;
switch(menu)
 {
  case ('1') :
      {
      cout<<" Nasgor "<<nama_menu;
      harga= 12000*jumbel ;
      }
      break;
  case ('2') :
      {
      cout<<" Bakso "<<nama_menu;
      harga= 15000*jumbel;
      }
      break;
  case ('3') :
      {
      cout<<"JUICE  "<<nama_menu;
      harga= 20000*jumbel;
      }
      break;
 }
cout<<endl;
cout<<" Harga Menu yang Anda Pesan    : Rp."<<harga<<endl;
    if (jumbel >5)
  {
   potongan = 0.3*harga;
  }
  else
  {
   potongan= 0;
  }
cout<<" Jumlah Menu yang Anda Pesan   : "<<jumbel<<endl;
cout<<" Total Harga                  : Rp."<<harga<<endl;
cout<<" Potongan Harga               : Rp."<<potongan<<endl;

totbay= harga-potongan;
cout<<" ---------------------------------------------"<<endl;
cout<<" Total Bayar                  : Rp."<<totbay<<endl;

cout<<" Bonus yang Anda Dapatkan     :"<<bns;
     if (jumbel >5)
  {
  cout<<"Aqua"<<bns;
  }
   else
  {
   cout<<"Maaf Tidak Dapat Bonus"<<bns;
  }
  cout<<endl;
cout<<" \n ";
cout<<"---------------------------------------------"<<endl;
cout<<"\t **** TERIMA KASIH ****        ";
cout<<endl;
cout<<" Apa Mau Input Data Lagi ? [Y/T] : ";cin>>yt;
cout<<endl;
clrscr();
if(yt=='Y' || yt=='y')
{goto kembali;}
if(yt=='T' || yt=='t')
{goto selesai;}
selesai:
cout<<endl;
cout<<"\t******* Terima Kasih *******"<<endl;
getch();
}
