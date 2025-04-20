# Tugas Flutter State Management dengan Streams

Mohamad Juan Adi Pratama - 1122140109

## Deskripsi Proyek

Proyek Flutter yang mendemonstrasikan state management dengan streams.

## Laporan Praktikum

### Soal no 1

Menambahkan nama panggilan pada title app sebagai identitas hasil pekerjaan dan mengganti warna tema sesuai kesukaan.

```dart
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Stream Juan',
      theme: ThemeData(primarySwatch: Colors.cyan),
      home: const StreamHomePage(),
    );
  }
```

### Soal no 2

Menambahkan 5 warna lainnya sesuai keinginan anda pada variabel colors

```dart
  final List<Color> colors = [
    Colors.blueGrey,
    Colors.amber,
    Colors.deepPurple,
    Colors.lightBlue,
    Colors.teal,
  ];
```

### Soal no 3

Jelaskan fungsi keyword yield\* pada kode tersebut

```dart
yield* Stream.periodic(const Duration(seconds: 1), (int t))
```

#### Penjelasan

yield/* berfungsi mengambil seluruh nilai dari stream yang direferensikan dan meneruskannya satu per satu ke stream yang sedang dibuat.

Apa maksud isi perintah kode tersebut?

```dart
  Stream<Color> getColors() async* {
    yield* Stream.periodic(const Duration(seconds: 1), (int t) {
      int index = t % colors.length;
      return colors[index];
    });
  }
```

#### Penjelasan

Kode ini membuat sebuah stream yang :
- Mengeluarkan warna dari array colors secara berurutan
- Berganti warna setiap 1 detik
- Setelah mencapai warna terakhir di array, kembali lagi ke warna pertama