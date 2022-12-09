Deleted issue #16 from https://github.com/mobigroup/gmtsar

## "zip-zip ура!"

Есть более сильные компрессоры общего назначения, чем Zip: https://github.com/IlyaGrebnov/libbsc
```
$ sha256sum -b 04f723-005.tiff 
f25d5c4a7c4fd1f3a04689c8d6f1142c1fabb6b622633050754d29af16b7dcb2 *04f723-005.tiff
$ du -b 04f723-005.tiff.* | sort
607257970	04f723-005.tiff.bsc  # -b2000 -t
700384091	04f723-005.tiff.zst
821559025	04f723-005.tiff.gz
```
Сравнимый с `bsc` результат вполне можно получить, написав простую специализированную утилиту, типа такой: https://github.com/alantudyk/yellow_briber/tree/master/dr10j, при этом скорость сжатия / распаковки — 0.2 GB/s и 1.0 GB/s соответственно.
