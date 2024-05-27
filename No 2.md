# NO 2
## Code cpp
```
#include <iostream>
#include <string>

class Mahasiswa {
    // Bagian private hanya dapat diakses oleh member functions dalam kelas ini
private:
    std::string nama;
    int umur;
    std::string prodi;
    std::string fakultas;

    // Bagian public dapat diakses dari luar kelas
public:
    // Konstruktor untuk menginisialisasi objek Mahasiswa
    Mahasiswa(std::string n, int u, std::string p, std::string f) {
        nama = n;
        umur = u;
        prodi = p;
        fakultas = f;
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

    // Setter untuk mengatur prodi
    void setProdi(std::string p) {
        prodi = p;
    }

    // Getter untuk mendapatkan prodi
    std::string getProdi() {
        return prodi;
    }

    // Setter untuk mengatur fakultas
    void setFakultas(std::string f) {
        fakultas = f;
    }

    // Getter untuk mendapatkan fakultas
    std::string getFakultas() {
        return fakultas;
    }

    // Metode untuk menampilkan informasi Mahasiswa
    void tampilkanInfo() {
        std::cout << "Nama: " << nama << ", Umur: " << umur << ", Prodi: " << prodi << ", Fakultas: " << fakultas << std::endl;
    }
};

int main() {
    // Membuat objek Mahasiswa
    Mahasiswa mhs("Lisa",20, "Guru", "keguruan dan ilmu pendidikan");

    // Menampilkan nama, umur, prodi, dan fakultas yang didapatkan dengan getter
    std::cout << "Nama: " << mhs.getNama() << std::endl;
    std::cout << "Umur: " << mhs.getUmur() << std::endl;
    std::cout << "Prodi: " << mhs.getProdi() << std::endl;
    std::cout << "Fakultas: " << mhs.getFakultas() << std::endl;

    return 0;
}
```

## Capture Hasil Running 
![Screenshot 2024-05-27 091119](https://github.com/euisjulianingsih/P11/assets/156889234/d3140f76-41cf-41e5-8f82-83a73f6f7a85)


