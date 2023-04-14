# Recent-Earthquakes
a=1
admin="barank"
adminparola="1234"

while(a==1):
    print("1- Giriş yap.\n2- Üye ol.\n3- Şifremi unuttum.\n4- Admin girişi.\n5- Çıkış yap.")
    secim=int(input("Lütfen seçim yapınız:"))
    if(secim==1):
        kullaniciadi=input("Kullanıcı adınızı giriniz:")
        parola=input("Şifrenizi giriniz:")
        if(kullaniciadi==yenikullanici and parola==yeniparola):
            print("\nSisteme hoş geldiniz!\n")
            print("menu")
        else:
            print("Kullanıcı adı veya şifre hatalı.")
             
    elif(secim==2):
        yenikullanici=input("Kullanıcı adı seçiniz:")
        yeniparola=input("Şifre seçiniz:")
        print("\nBaşarıyla kaydoldunuz!\n")
        
    elif(secim==3):
        k1=input("Kullanıcı adınızı giriniz:")
        if(k1==yenikullanici):
            print("Şifreniz:",yeniparola)
        elif(k1=="barank"):
            print("\nŞifreniz:",adminparola,"\n")
            
    elif(secim==4):
        kadmin=input("Kullanıcı adınızı giriniz:")
        padmin=input("Şifrenizi giriniz:")
        if(kadmin==admin and padmin==adminparola):
            print("Sisteme hoş geldiniz!")
            print("adminmenusu")
        else:
            print("Kullanıcı adı veya şifre hatalı.")
    elif(secim==5):
        print("Çıkış yapılıyor...")
        a=2
    
    else:
        print("Geçersiz giriş yaptınız. Tekrar deneyin.")
