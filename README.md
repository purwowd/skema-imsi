# skema-imsi
Skema IMSI operator seluler di Indonesia

###  1. **Telkomsel** 
- `510 10 AB CD EF GH IJ`
  | skema | keterangan |
  |---|---|
  | 510| Kode MCC untuk tsel (kode negara seluler) |
  | 10 | Kode MNC untuk tsel (kode jaringan seluler) |
  | AB | Awalan untuk HLR (berisi informasi pelanggan seluler sesuai arsitektur GSM) |
  | C | NDC (kode tujuan nasional) |
  | D | Identitas produk (ID: Halo, Simpati, AS, etc) |
  | EFGHIJ | Nomor urut untuk IMSI dan ICCID |
  | Jumlah | **15** digit |

- **Contoh**: `510107032343835`
  | imsi | keterangan |
  |---|---|
  | 510| Kode negara seluler untuk tsel |
  | 10 | kode jaringan seluler untuk tsel |
  | 70 | Awalan untuk HLR (10 - 99) |
  | 3 | Kode Tujuan Nasional (0813) |
  | 2 | Identitas produk (kartu simpati) |
  | 343835 | Nomor urut untuk IMSI dan ICCID |

  ```bash
  (skema-imsi) ➜ python imsi_to_msisdn.py 
  input your imsi: 510107032343835
  => 081370343835 <=
  ```

### 2. **XL Axiata / AXIS**
- `510 11` => ??

### 3. **Indosat Ooredoo**
- `510 01` => ??
