# FINAL TASLAK
Bu repo [Patike.dev](https://www.patika.dev/) tarafindan gerceklestirilen AKBANK COBOL COOTCAMP'i icin final odevinin taslagidir.


![jpeg](https://github.com/CheaterAK/COBOL-TASLAK/blob/master/resim.jpg?raw=true)
---
## Calisma sirasinda kullanilan dosyalar

Programimiz toplam 3 dosya ile calismaktadir. 
```
Idxfile: VSAM dosyasi icerisinde kullanici bilgileri bulunur.
Inpfile: QSAM dosyasi icerisinde kullanici bilgilerine ulsamak icin key bulunur.
Outfile: QSAM dosyasi alt programdan gelen degere gore yapilan islemleri loglar.
```
Bunlar haricinde bir sysout ve birde syserr bulunmakta bunlar terminala verilen ciktilardir.
```
sysout: Read edilen datada ne var ise tamamini yazdirir.
syserr: Inpfile da bulunan hatalardan kaynakli mesajlar buraya cikarilmaktadir.
```

## Ana mantik

```
Ana program Idxfile haricinde tum dosyalari acar.
Inpfiledan bir satir okur bu satirin uygunlugunu degerlendirir eger uygun ise alt programa gonderir.
Alt program Inpfiledan gelen key ile vsamdaki kayda ulasir ve uygun islem tipindeki calismayi uygular.
alt programdan donen bilgiler ile ana programda cikti uretilip out file a yazilir.
```

