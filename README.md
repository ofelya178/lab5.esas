n = int(input("Massivin uzunluğunu daxil edin: "))
C = [int(input(f"Element {i+1}: ")) for i in range(n)]

uygun_elementler = [eleman for eleman in C if eleman % 3 == 2]

if uygun_elementler:
    ortalama = sum(uygun_elementler) / len(uygun_elementler)
    print("Ortalamalar: ", ortalama)
else:
    print("3-ə bölünəndə qalıqda 2 olan element tapılmadı")
