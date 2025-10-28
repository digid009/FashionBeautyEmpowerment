# --- Syarat 4: OOP (Object-Oriented Programming) ---
class Peserta:
    """Menyimpan data peserta dan level kepercayaan diri."""
    def __init__(self, nama, pd_awal=5):
        self.nama = nama
        self.level_pd = pd_awal
        self.keterampilan_modul = []

    def tampilkan_profil(self):
        print(f"\n✨ Profil {self.nama}:")
        print(f"   Level Kepercayaan Diri: {self.level_pd}/10")
        print(f"   Modul Selesai: {len(self.keterampilan_modul)}")

    def tingkatkan_pd(self, modul):
        """Method untuk meningkatkan PD dan mencatat modul."""
        self.level_pd += 1
        self.keterampilan_modul.append(modul)

# --- Syarat 3: Function (Fungsi Mandiri) ---
def berikan_motivasi(level):
    """Memberikan kata-kata motivasi berdasarkan level PD peserta."""
    # --- Syarat 1: If Statement ---
    if level < 7:
        return "Teruslah belajar! Setiap keterampilan kecil akan membangun kepercayaan diri yang besar. Anda luar biasa!"
    elif level >= 7 and level < 10:
        return "Kepercayaan diri Anda sudah sangat baik! Terus pancarkan pesona diri Anda yang unik!"
    else: # level 10 atau lebih
        return "Anda adalah ikon! Dunia siap melihat potensi dan gaya terbaik Anda!"

# Fungsi utama program
def main():
    print("=========================================")
    print(" PROGRAM FASHION & BEAUTY EMPOWERMENT 🚀")
    print("=========================================")

    nama_user = input("Masukkan nama Anda untuk mendaftar: ")
    peserta_aktif = Peserta(nama_user) # Objek peserta dibuat

    modul_pembelajaran = ["Styling Dasar", "Basic Makeup", "Perawatan Diri", "Komunikasi Positif"]

    # --- Syarat 2: While Loop untuk Menu Utama ---
    while True:
        print("\n--- MENU ---")
        print("1. Ikuti Modul Pembelajaran")
        print("2. Cek Level Kepercayaan Diri")
        print("3. Keluar Program")

        pilihan = input("Pilih aksi (1/2/3): ")

        # --- Syarat 1: If Statement untuk Navigasi ---
        if pilihan == '1':
            print("\nAnda akan memulai proses pembelajaran:")
            
            # --- Syarat 2: For Statement untuk Modul ---
            for i, modul in enumerate(modul_pembelajaran):
                print(f"Modul {i+1}: Sedang mempelajari **{modul}**...")
                peserta_aktif.tingkatkan_pd(modul) # Memanggil method dari objek
            
            print("\n🎉 Semua modul selesai! Kepercayaan diri Anda meningkat.")

        elif pilihan == '2':
            peserta_aktif.tampilkan_profil()
            motivasi = berikan_motivasi(peserta_aktif.level_pd) # Memanggil fungsi mandiri
            print(f"\nKata Motivasi: {motivasi}")

        elif pilihan == '3':
            print(f"\nSampai jumpa, {peserta_aktif.nama}! Ingat, percaya diri adalah outfit terbaik Anda. 👋")
            break # Keluar dari While Loop

        else:
            print("Pilihan tidak valid. Silakan coba lagi.")

if __name__ == "__main__":
    main()
