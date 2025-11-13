# AutoMath_Project
    print("Kalkulator Sederhana")
    print("Operasi: + (tambah), - (kurang), * (kali), / (bagi)")
    
    try:
        num1 = float(input("Masukkan angka pertama: "))
        operasi = input("Masukkan operasi (+, -, *, /): ")
        num2 = float(input("Masukkan angka kedua: "))
        
        if operasi == '+':
            hasil = num1 + num2
        elif operasi == '-':
            hasil = num1 - num2
        elif operasi == '*':
            hasil = num1 * num2
        elif operasi == '/':
            if num2 == 0:
                print("Error: Tidak bisa membagi dengan nol!")
                return
            hasil = num1 / num2
        else:
            print("Operasi tidak valid!")
            return
        
        print(f"Hasil: {num1} {operasi} {num2} = {hasil}")
    except ValueError:
        print("Error: Masukkan angka yang valid!")
# Jalankan kalkulator
kalkulator()
