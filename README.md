
[Patika](www.patika.dev)

# Degiskenler C# console projesi ilk Ödev

       ''' using System;
        
        namespace degiskenler  {
        
        class Program    {
        
        private static void Main(string[] args) {
        
        Console.WriteLine("Kosol Programlama C# Ilk Ödev");
        
   '''

###  // Stringlerde neler yapabiliriz, String Ifade sekilleri

      Bos String tanimala sekilleri : 
      
      Gösterim 1 : 'string? str1 = "" '
      Gösterim 2 : ' string? str1 = null;'

    
        Gösterim 3 Bos String tanimlama
      
        'string? str1 =string.Empty;'
        
       'str1 = "Celale Yildiz Yazar" ;  // String e deger atamak istiyorsak:'
        
      '''string? ad = " Celale";
       
       string? soyad = " Yildiz Yazar ";

      string? tamlsin = ad + " " +soyad;  // Stringleri birlestirme yollarindan biri bu sekilde.'''

### // Integer tanimlama sekilleri
  'int integer1 = 5;'
  'int integer2 = 3;'
  'int integer3 = integer1 * integer2;'

### // boolean ifade tanimlama sekilleri 
'bool bool1 = 10<2'

###   DEGISKENLERIN BIRBIRLERINE DÖNUSUMLERI

#### String Dönüsümleri: Örnegin bir String ifadenin  bir intger ifadesiyle birlestirilip yeni bir string deger elde etmek isitiyoruz:
     '''string? str20 = "20";
       int int20 = 20;
       string? yeniDeger = str20 + int20.ToString();
       Console.WriteLine(yeniDeger); // Ciktisi 2020 ,terminale gidip bak.'''

#### Integer Dönüsümleri : Örnegin Bir Integer degerin bir Örnegin bir String deger ile birlestirilip matematiksel toplayip yeni bir integer deger elde etmek istiyoruz.

        ''' int int21 = int20 + Convert.ToInt32(str20);
        
           Console.WriteLine(int21); // Ciktisi 40 '''

Convert fonksiyonlarinin yanisira .Aynizamanda degsim yapabilcegimiz diger  bir fonskiyon Parse, ama  Parse ile sadece string degerler icin kullaniliyor.

    'int int22 = int20 + int.Parse(str20); //ciktisi 40 olacak'

### Datetime dönüsümleri

   '''string? datetime = DateTime.Now.ToString("dd.MM.yyyy");  // Bir Datetime ciktiyi string dönüsütür ve verirken bunu formatla, normalde saatle birlikte                                                                               tarihgeliyor
          Console.WriteLine(datetime);                   // ama ben saat gelsin istemiyoru, sadece gün, ay, yil olarak aralarinda nokta ile getir. '''

peki tarihlerin arasinda nokta degil / olsun olarak istersem 

          ''' string? datetime2 = DateTime.Now.ToString("dd/MM/yyyy"); 
         // Bir Datetime ciktiyi string dönüsütür ve verirken bunu formatla, normalde saatle birlikte tarihgeliyor
          Console.WriteLine(datetime2);'''  

// bu tarihteki saati de ayrica almak istiyorsak

          ''' string? hour = DateTime.Now.ToString("HH:mm");
             Console.WriteLine(hour);
        
 
        }
    }
}

'''
