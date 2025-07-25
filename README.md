# tas_kagit_makas.py
3.denemem
import random
liste=["tas","kagit","makas"]
liste2=["makas","kağıt","kagit","tas","taş"]
while True:
    a=input("Tas mi kagit mi makas mi?,cikis icin q basiniz: ").lower().strip()
    if a=="q":
        break
    elif a  not in liste2:
        print("Gecersiz islem!")
        continue
    else:
        secim=random.choice(liste)
        if (a=="taş" or a=="tas") and secim=="makas":
            print(f"sizin seciminiz {a}, bilgisayarin secimi {secim},Siz kazandiniz!")
        elif (a=="taş" or a=="tas") and secim=="kagit":
            print(f"sizin seciminiz {a}, bilgisayarin secimi {secim},Bilgisayar kazandi...")
        elif (a=="taş" or a=="tas") and secim=="taş":
            print(f"sizin seciminiz {a}, bilgisayarin secimi {secim},Berabere")
        elif (a=="makas") and secim=="kagit":
            print(f"sizin seciminiz {a}, bilgisayarin secimi {secim},Siz kazandiniz!")
        elif (a=="makas") and secim=="tas":
            print(f"sizin seciminiz {a}, bilgisayarin secimi {secim},Bilgisayar kazandi...")
        elif (a=="makas") and secim=="makas":
            print(f"sizin seciminiz {a}, bilgisayarin secimi {secim},Berabere")
        elif (a=="kağıt" or a=="kagit") and secim=="tas":
            print(f"sizin seciminiz {a}, bilgisayarin secimi {secim},Sen kazandin!")
        elif (a=="kağıt" or a=="kagit") and secim=="makas":
            print(f"sizin seciminiz {a}, bilgisayarin secimi {secim},Bilgisayar kazandi...")
        elif (a=="kağıt" or a=="kagit") and secim=="kagit":
            print(f"sizin seciminiz {a}, bilgisayarin secimi {secim},Berabere")





