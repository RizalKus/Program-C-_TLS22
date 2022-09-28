# Program-C-_TLS22
Rizal Kurniawan Saputra
OHM

#include <iostream>

using namespace std;

int main()
{
    
    
   string nama;
   double bb, tb, bmi, u, n;
   int bmaks, bmin;
   

    cout<<"##       Program Menghitung Berat Badan Ideal        ##"<<endl;
    cout<<endl;
    cout<<"Masukkan jumlah orang yang mau diukur: ";
    cin>>n;
    cout<<"============================================================="<<endl;
    for(int i=1;i<=n;i++){
        cout<<"Masukkan nama                : ";
        cin>>nama;
        cout<<"Berat badan(kg) orang ke-"<<i<<"   : ";
        cin>>bb;
        cout<<"Masukkan tinggi(meter)       : ";
        cin>>tb;
        cout<<"Masukkan usia(tahun)         : ";
        cin>>u;
        bmi=bb/(tb*tb);
        cout<<"\nBody Mass Index(BMI) Anda adalah "<<bmi<<endl;
        cout<<endl;
        
    if (bmi<=18.5){
    cout<<"Keterangan: Anda kekurangan berat badan"<<endl; 
    } else if (bmi>18.5 && bmi<=25){
    cout<<"Keterangan: Berat badan Anda ideal"<<endl;
    } else if (bmi>25 && bmi<=30){
    cout<<"Keterangan: Anda kelebihan berat badan"<<endl;
    } else {
    cout<<"Keterangan: Anda obesitas"<<endl;
    }
    cout<<endl;
    
    cout<<"++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++"<<endl;
    cout<<"             PATOKAN MINIMAL & MAKSIMAL           "<<endl;
    cout<<"Tinggi Badan (meter)                     = "<<tb<<endl;
    
    double min=18.4;
    bmin=min*tb*tb;
    cout<<"Berat badan(kg) ideal minimal            = "<<bmin<<endl;
    double maks=24.9;
    bmaks=maks*tb*tb;
    cout<<"Berat badan(kg) ideal maksimal           = "<<bmaks<<endl;
    cout<<"+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++"<<endl;
    cout<<endl;
    }
   
    return 0;
}
