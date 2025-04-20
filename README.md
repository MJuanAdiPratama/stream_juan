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