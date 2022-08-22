[Patika.dev](https://github.com/mordulu)


Dosyalarımın içinde yer alan program.cs'ye girilme zahmeti olmaması adına aşağıya çalışmamı önizleme olarak ekliyorum(süslü parantezler önizlemede hata verdiğinden konumlandırmalarına dikkat etmeyiniz)


# Değişkenler - Ders Notları

         using System;

         namespace degisken
         {

        class Program
 
        {
    
        static void Main(string[] args)
         {
        Console.WriteLine("");
        String degisken = " ";
        byte b = 5;  //0 ila 255 arası değer alabilir         1 byte yer kaplar
        sbyte c =5;   //-128 ila 127 arası değer alabilir     1 byte yer kaplar

        short s = 5;  //-32768 ila 32768 arası değer alabilir 2 byte yer kaplar
        ushort us =5; //0 ila 65365 arası değer alabilir      2 byte yer kaplar

        Int16 i16 = 2; // 2 byte yer kaplar
        int i =2;      // -2000147483648 ila + karşılığı      2 byte yer kaplar
        Int32 i32 = 2; // 4 byte yer kaplar
        Int64 i64 =2;  // 8 byte yer kaplar


        //Reel Sayılar

        uint ui = 2;  //4 byte
        long l = 4;   //8 byte
        ulong ul = 4; //8 byte

        float f = 5;   //4 byte
        double d = 5;  //8 byte
        decimal de = 5; //16 byte

        char ch = '2';
        string str ="Melih"; //sınırsız
        
        bool b1 = true;
        bool b2 = false;

        DateTime dt= DateTime.Now;

        Console.WriteLine(dt);

        object o1 = "x";
        object o2 = "y";
        object o3 = 4;
        object o4 = 4.3;

        // string ifadeler

        string str1 = string.Empty;
        str1 = "Melih Ordulu";
        string ad = "Melih";
        string soyad = "Ordulu";
        string tamisim = ad + " " +soyad;

        //integer tanımlama şekilleri

        int integer1 = 5;
        int integer2 = 3;
        int integer3 = integer1 * integer2;

        //boolean

        bool bool1 = 10>2;

        // Değişken Dönüşümleri

        string str20 = "20";
        int int20 = 20;

        string yeniDeğer = str20 + int20.ToString();

        Console.WriteLine(yeniDeğer);

        int int21 = int20 + Convert.ToInt32(str20);
        Console.WriteLine(int21); // Çıktısı 40 

        int int22 = int20 + int.Parse(str20);   //Çıktısı 40

        // datetime

        string datetime = DateTime.Now.ToString("dd.MM.yyyy");
        Console.WriteLine(int21); 

        string datetime2 = DateTime.Now.ToString("MM/dd/yyyy");
        Console.WriteLine(datetime2); 

        string hour = DateTime.Now.ToString("HH.mm");
        Console.WriteLine(hour); 
