---
title: Model
description: ''
position: 5 
category: Medical Record
---
<style>
td, th {
   border: none!important;
}
.prose thead{
    border-bottom-width: 0px !important;
}
</style>

## Intro
Dokumen ini menampung bagaiman data pada medical record disimpan. Pada `API` untuk menyimpan data `MedicalRecord` dengan menunjukkan skema request seperti berikut:
```json
[
  {
    "device_id":"11:FF",
    "member_id":"dsdfs",
    "nurse_id":"sada",
    "type":"HEART_RATE",
    "value":"80",
    "method":"AUTOMATIC",
    "created_at":0,
    "assets":"ini asset",
    "diagnosis":"diagnosis",
    "note":"ini adalah note",
    "title":"bpm",
    "mime_type":"text"
  }
]
```
Seperti yang terlihat pada data diatas untuk menyimpan data medical record terdapat pada `value` karena setiap data memiliki perbedaan maka kita menyimpan datanya dalam bentuk json untuk contoh diatas adalah medical record yang memilik 1 value maka akan langsung diisi seperti diatas, sedangkan untuk data yang memilik lebih dari 1 value akan diubah menjadi data json. Anda dapat melihat schemanya pada dokumentasi ini.

## Skema

### Body Mass Index

| Name       | description |
|------------|-------------|
| weight   |   float         |
| height  |     float        |

Contoh:
```json5
  {
    ...
    "value":{
        "weight":80,
        "height":90
    }
    ...
  }
```

### Blood Pressure

| Name       | description |
|------------|-------------|
| systole   |   int          |
| diastole  |     int        |

Contoh:
```json5
  {
    ...
    "value":{
        "systole":80,
        "diastole":90
    }
    ...
  }
```

### Blood Oxygen

| Name       | description |
|------------|-------------|
| spo2   |   int          |

Contoh:
```json5
  {
    ...
    "value":{
        "systole":80,
        "diastole":90
    }
    ...
  }
```

### Heart Rate

| Name       | description |
|------------|-------------|
| value   |   int          |

Contoh:
```json
  {
    ...
    "value":85
    ...
  }
```

### Heart Rate

| Name       | description |
|------------|-------------|
| value   |   int          |

Contoh:
```json
  {
    ...
    "value":85
    ...
  }
```

### Waist

| Name       | description |
|------------|-------------|
| value   |   int          |

Contoh:
```json
  {
    ...
    "value":85
    ...
  }
```

### Pedometer

| Name       | description |
|------------|-------------|
| value   |   int          |

Contoh:
```json
  {
    ...
    "value":85
    ...
  }
```

### Temperature

| Name       | description |
|------------|-------------|
| value   |   int          |

Contoh:
```json
  {
    ...
    "value":85
    ...
  }
```