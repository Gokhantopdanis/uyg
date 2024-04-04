# PASS1 ALGORİTMASINI YÜKSEK SEVİYELİ DİLDE YAZMAK

## 1.Adım
Boş bir sembol dizisi oluşturulur ve bulunduğu kodum 0 olarak ayarlanır.<br>
`sembol_tablosu = {} ` <br>
`location_counter = 0 `
## 2.Adım
dosyayı okunur satır sonu karakterlerini kaldır ve bş satıları kaldırılır. <br>
`with open(input_file, 'r') as file:` <br>
        `for line in file:`<br>
            `line = line.strip() `<br>
            `if not line:`<br>
                `continue`
## 3.Adım
Etiket, komut ve operandı ayrılır
`ayir = line.split()`
`label = ayir[0]`
`opcode = ayir[1]`
`operand = ayir[2] if len(ayir) > 2 else None`
## 4.Adım
Etiket var mı yok mu kontrol edilir
`if label: 
 sembol_tablosu[label] = location_counter`
## 5.Adım
kommutun boyutu belirlenir
``
