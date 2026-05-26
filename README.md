# Tugas-spam
Program filter email 
# ==========================================
# PROGRAM FILTER EMAIL SPAM
# ==========================================

print("=" * 10, "FILTER EMAIL SPAM", "=" * 10)

# Kata yang sering muncul di email spam
kata_spam = {"promo", "diskon", "hadiah", "gratis", "bonus"}

# Isi email
email = input("Masukkan isi email: ").lower()

# Ubah email menjadi set kata
kata_email = set(email.split())

# Cek kata yang cocok
hasil = kata_email.intersection(kata_spam)

# Output
print("\nKata spam yang ditemukan:", hasil)

if hasil:
    print("Status: Email kemungkinan besar SPAM")
else:
    print("Status: Email aman / bukan spam")
