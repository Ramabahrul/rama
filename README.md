TUGAS 1 

#include <iostream>
using namespace std;

double menghitungkinetik;

void hitungEK(double massa, double kecepatan) {
	menghitungkinetik = 0.5 * massa * kecepatan * kecepatan;
}

int main() {
	double massa, kecepatan, energiKinetik;

	cout << "Masukkan massa total dari sepeda + berat andi: ";
	cin >> massa;
	cout << "Masukkan kecepatan: ";
	cin >> kecepatan;


	hitungEK(massa, kecepatan);
	cout << "Energi kinetik: " << menghitungkinetik << endl;

	return 0;
}





TUGAS 2



#include <iostream>
#include <iomanip>

using namespace std;

int main() {
    
    double beratApel, beratJeruk, beratSemangka, totalBerat, totalHarga, diskon;
    const double hargaApel = 24000, hargaJeruk = 16250, hargaSemangka = 8000;

    
    cout << "Masukkan berat apel (kg): ";
    cin >> beratApel;
    cout << "Masukkan berat jeruk (kg): ";
    cin >> beratJeruk;
    cout << "Masukkan berat semangka (kg): ";
    cin >> beratSemangka;

    
    totalBerat = beratApel + beratJeruk + beratSemangka;
    totalHarga = (beratApel * hargaApel) + (beratJeruk * hargaJeruk) + (beratSemangka * hargaSemangka);

    
    if (totalBerat > 10) {
        diskon = 0.05;
    }
    else if (totalBerat > 8) {
        diskon = 0.02;
    }
    else {
        diskon = 0;
    }

    
    double totalBayar = totalHarga - (totalHarga * diskon);

    
    cout << fixed << setprecision(2);
    cout << "Total yang harus dibayar: Rp " << totalBayar << endl;

    return 0;
}
