# NO 1
## code cpp

```
#include <iostream>
#include <string>

class Mahasiswa {
    // Bagian private hanya dapat diakses oleh member functions dalam kelas ini
private:
    std::string nama;
    int umur;

    // Bagian public dapat diakses dari luar kelas
public:
    // Konstruktor untuk menginisialisasi objek Mahasiswa
    Mahasiswa(std::string n, int u) {
        nama = n;
        umur = u;
    }

    // Setter untuk mengatur nama
    void setNama(std::string n) {
        nama = n;
    }

    // Getter untuk mendapatkan nama
    std::string getNama() {
        return nama;
    }

    // Setter untuk mengatur umur
    void setUmur(int u) {
        umur = u;
    }

    // Getter untuk mendapatkan umur
    int getUmur() {
        return umur;
    }

    // Metode untuk menampilkan informasi Mahasiswa
    void tampilkanInfo() {
        std::cout << "Nama: " << nama << ", Umur: " << umur << std::endl;
    }
};

int main() {
    // Membuat objek Mahasiswa
    Mahasiswa mhs("Mark", 20);

    // Menggunakan metode public untuk mengakses data private
    std::cout << "Informasi awal Mahasiswa:" << std::endl;
    mhs.tampilkanInfo();

    // Mengubah nama dan umur menggunakan setter
    mhs.setNama("chanyeol");
    mhs.setUmur(21);

    // Menampilkan informasi yang sudah diubah
    std::cout << "informasi setelah diubah:" << std::endl;
    mhs.tampilkanInfo();

    std::cout << "Nama:" << mhs.getNama() << std::endl;
    std::cout << "Umur:" << mhs.getUmur() << std::endl;

    return 0;
}
```

### Capture Hasil Running 
![Screenshot 2024-05-27 090812](https://github.com/euisjulianingsih/P11/assets/156889234/f40dcd0e-8df7-4961-aaa5-f44e686d4f83)
