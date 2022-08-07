# shop
produkt1_name = input("Produkt name :")

preis_produkt1 = input("Preis:")

preis_produkt1_flt = float(preis_produkt1)

produkt1_frage = input("Ist ihr Produkt Lebensmittel('y' eingeben) oder Essen(irgendwas eingeben) ? ")

if  produkt1_frage == "y" :
    preis_produkt1_flt_brto = preis_produkt1_flt-preis_produkt1_flt*0.07
    Rechnung_Lm = input("Rechnung berechnen? ")

    if  Rechnung_Lm == "ja" :
        print(str(preis_produkt1_flt) + " €(netto)")
        print(str(preis_produkt1_flt_brto) + " €(brutto)")
        
    else  :
        produkt2_name = input("Produkt name : ")
        preis_produkt2 = input("Preis:")
        preis_produkt2_flt = float(preis_produkt2)
        produkt2_frage = input("Ist ihr Produkt Lebensmittel('y' eingeben) oder Essen(irgendwas eingeben) ? ")
        if  produkt2_frage == "y" :
            preis_produkt2_flt_brto = preis_produkt2_flt-preis_produkt2_flt*0.07
            Rechnung_Lm_2 = input("Rechnung berechnen? ")

            if Rechnung_Lm_2 == "ja" :
                Endpreis2 = preis_produkt1_flt + preis_produkt2_flt
                Endpreis2_str = str(Endpreis2)
                print( Endpreis2_str + " €(netto)")
                Endpreis2_brto = preis_produkt1_flt_brto +  preis_produkt2_flt_brto 
                Endpreis2_str_brto = str(Endpreis2_brto)
                print( Endpreis2_str_brto + " €(brutto)")

            else  :
                print("hzm")

        else :
            print("hzm3")
            



else  :
    preis_produkt1_flt_brto = preis_produkt1_flt-preis_produkt1_flt*0.16
    Rechnung1_essen = input("Rechnung berechnen? ")
    
    if  Rechnung1_essen == "ja" :
        print(str(preis_produkt1_flt) + " €(netto)")
        print(str(preis_produkt1_flt_brto) + " €(brutto)")
        
    else  :
        #test
        produkt2_name = input("Produkt name : ")
        preis_produkt2 = input("Preis:")
        preis_produkt2_flt = float(preis_produkt2)
        produkt2_frage = input("Ist ihr Produkt Lebensmittel('y' eingeben) oder Essen(irgendwas eingeben) ? ")
        if  produkt2_frage == "y" :
            preis_produkt2_flt_brto = preis_produkt2_flt-preis_produkt1_flt*0.16
            Rechnung2 = input("Rechnung berechnen? ")

            if Rechnung2 == "ja" :
                Endpreis2 = preis_produkt1_flt + preis_produkt2_flt
                Endpreis2_str = str(Endpreis2)
                print( Endpreis2_str + " €(netto)")
                Endpreis2_brto = preis_produkt2_flt_brto + preis_produkt1_flt_brto
                Endpreis2_str_brto = str(Endpreis2_brto)
                print( Endpreis2_str_brto + " €(brutto)")


            else  :
                print("hzm16") 

        else :
            print("hzm3")




