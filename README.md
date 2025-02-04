# 🧬 Genetic Algorithm for Function Optimization  

![Genetic Algorithm](https://bs-uploads.toptal.io/blackfish-uploads/components/open_graph_image/8958295/og_image/optimized/0901-Genetic_Algorithms-Search_and_Optimization_by_Natural_Selection_Dan_Social-c593a24c34612eaba65058efa44e7980.png)

## 🔍 Overview
Proyek ini mengimplementasikan **Genetic Algorithm (GA)** untuk menemukan nilai optimal dari fungsi matematika tertentu. GA adalah metode optimasi berbasis evolusi yang meniru seleksi alam, di mana individu terbaik bertahan dan bereproduksi untuk menghasilkan solusi optimal.  

## 🎯 Objective
- Mencari nilai **x₁** dan **x₂** yang menghasilkan nilai minimum dari fungsi matematika yang diberikan.  
- Menggunakan **Genetic Algorithm** dengan metode **Tournament Selection, Crossover, dan Mutation**.  

## 🛠️ Metode & Implementasi
### **1️⃣ Inisialisasi Parameter**
- **Ukuran populasi**: 100 individu  
- **Panjang kromosom**: 20 bit  
- **Probabilitas crossover (Pc)**: 0.6  
- **Probabilitas mutasi (Pm)**: 0.1  
- **Batas domain variabel**: `[-10, 10]`  

### **2️⃣ Representasi Kromosom**
- Setiap individu dalam populasi direpresentasikan sebagai **string biner** yang dikonversi menjadi nilai numerik menggunakan **decoding function**.  

### **3️⃣ Seleksi Orang Tua (Tournament Selection)**
- **5 individu acak** dipilih dari populasi.  
- Individu dengan **fitness value** terbaik akan dipilih untuk crossover.  

### **4️⃣ Crossover & Mutasi**
- **Crossover (Pindah Silang):**  
  - **One-point crossover** digunakan untuk menggabungkan gen dari dua individu.  
  - Probabilitas crossover **60%**.  
- **Mutasi:**  
  - Mutasi terjadi dengan **probabilitas 10%** untuk memperkenalkan variasi dalam populasi.  

### **5️⃣ Evaluasi & Seleksi Generasi Baru**
- **Fitness Function** digunakan untuk mengevaluasi setiap individu.  
- **Generational Replacement** digunakan untuk menggantikan populasi lama dengan individu baru.  

## 📊 Hasil Eksperimen
- Metode terbaik: Tournament Selection + Generational Replacement
- Solusi optimal: Nilai x₁ dan x₂ yang memberikan minimum fungsi target
- Fitness function menunjukkan konvergensi yang stabil setelah beberapa generasi.

## 🛠️ Teknologi & Tools
- 🐍 Python
- 📦 NumPy, Pandas, Matplotlib
- 🤖 Scikit-learn
- 📊 Google Colab

## 📜 Referensi
1. Goldberg, D. E. (1989). Genetic Algorithms in Search, Optimization & Machine Learning.
2. Mitchell, M. (1996). An Introduction to Genetic Algorithms.
