# Tugas-W10
# def huruf_ke_angka(huruf):
def huruf_ke_angka(huruf):
    return ord(huruf.upper()) - ord('A') + 1
def proses_nama(nama):
    nama = nama.replace(" ", "") 
    if len(nama) < 3:
        return "Nama terlalu pendek."
    huruf_pertama = nama[0]
    huruf_terakhir = nama[-1]
    huruf_tengah = nama[len(nama) // 2]
    angka1 = huruf_ke_angka(huruf_pertama)
    angka2 = huruf_ke_angka(huruf_tengah)
    angka3 = huruf_ke_angka(huruf_terakhir)
    total = angka1 + angka2 + angka3
    print(f"Huruf pertama : {huruf_pertama} -> {angka1}")
    print(f"Huruf tengah  : {huruf_tengah} -> {angka2}")
    print(f"Huruf terakhir: {huruf_terakhir} -> {angka3}")
    print(f"Total nilai   : {total}")
    return total
proses_nama("Hourisa Zukhrufiana")
