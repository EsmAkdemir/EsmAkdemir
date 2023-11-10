# JSON'dan CSV'ye Dönüştürme Programı

Bu C programı, JSON formatındaki verileri okuyarak bu verileri CSV (Comma-Separated Values) formatına dönüştürmek için kullanılır.

## Kullanım


Programı çalıştırmak için terminal veya komut istemcisinde aşağıdaki komutu kullanabilirsiniz:

```
$ ./program <JSON dosya adı> <CSV dosya adı> <header=ON|OFF>
```

<JSON dosya adı>: Dönüştürmek istediğiniz JSON dosyasının adı. </br>
<CSV dosya adı>: Dönüştürülen verilerin kaydedileceği CSV dosyasının adı. </br>
<header=ON|OFF>: CSV dosyasına başlık eklemek istiyorsanız ON, eklemek istemiyorsanız OFF. </br> 


## **Örneğin** 

``` 
$ ./program input.json output.csv header=ON 
```

Bu komut, 'input.json' adlı JSON dosyasını okuyacak, verileri 'output.csv' adlı CSV dosyasına dönüştürecek ve başlığı CSV dosyasına ekleyecektir.

## Programın Çalışma Mantığı
Program, JSON formatındaki verileri okuyarak öğrenci bilgilerini içeren bir yapı oluşturur. JSON dosyasındaki öğrenci verileri şu şekildedir:
```
[
    {
        "id": 1, 
        "name": "Ahmet Yilmaz", 
        "grades": { 
            "midterm": 75, 
            "final": 85 
        }, 
        "course": "BIL 203" 
    },
    {
        "id": 2,
        "name": "Ayse Kaya",
        "grades": {
            "midterm": 80,
            "final": 88
        },
        "course": "BIL 203" 
    },
    {
        "id": 3,
        "name": "Mehmet Demir",
        "grades": {
            "midterm": 70,
            "final": 82
        },
        "course": "BIL 203"
    }
]
```

Program, JSON dosyasını okuyarak öğrenci bilgilerini alır, bunları bir CSV dosyasına dönüştürür ve isteğe bağlı olarak başlığı ekler.

## Geliştirme ve Katkı
Eğer bu projeye katkıda bulunmak isterseniz, lütfen forklayın ve pull request açın. Her türlü katkıya açığız.

