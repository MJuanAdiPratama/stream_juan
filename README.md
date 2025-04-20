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