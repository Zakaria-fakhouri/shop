# shop
list_P = [ ]

P = input("podukt eingeben : ")
r = input("Preis: ")
pr = float(r)
fr = input("Ist ihr Produkt Lebensmittel('ja' eingeben) oder Essen(irgendwas eingeben) ? ")

list_P.insert(0, P)

if fr == "ja":
  pr_bro = pr-pr*0.07

else:
  pr_bro = pr-pr*0.16    

re = input("Rechnung berechnen? ")

if re == "ja":
  print(("warenkorb: ") + str(list_P))
  print(("preis(netto): ") + str(pr))
  print(("preis(brutto): ") + str(pr_bro))

else:
    P = input("podukt eingeben : ")
    r2 = input("Preis: ")
    pr2 = float(r2)
    fr = input("Ist ihr Produkt Lebensmittel('ja' eingeben) oder Essen(irgendwas eingeben) ? ")
    list_P.insert(1, P)
    if fr == "ja":
      pr2_bro = pr2-pr2*0.07

    else:
      pr2_bro = pr2-pr2*0.16    

    re = input("Rechnung berechnen? ")

    if re == "ja":
       print(("warenkorb: ") + str(list_P))
       print(("preis(netto): ") + str(pr + pr2))
       print(("preis(brutto): ") + str(pr_bro + pr2_bro))

    else:
       P = input("podukt eingeben : ")
       r3 = input("Preis: ")
       pr3 = float(r3)
       fr = input("Ist ihr Produkt Lebensmittel('ja' eingeben) oder Essen(irgendwas eingeben) ? ")
       list_P.insert(2, P)

       if fr == "ja":
        pr3_bro = pr3-pr3*0.07

       else:
        pr3_bro = pr3-pr3*0.16    

       re = input("Rechnung berechnen? ")

       if re == "ja":
        print(("warenkorb: ") + str(list_P))
        print(("preis(netto): ") + str(pr + pr2 + pr3))
        print(("preis(brutto): ") + str(pr_bro + pr2_bro + pr3_bro))

       else:
        P = input("podukt eingeben : ")
        r4 = input("Preis: ")
        pr4 = float(r4)
        fr = input("Ist ihr Produkt Lebensmittel('ja' eingeben) oder Essen(irgendwas eingeben) ? ")
        list_P.insert(3, P)

        if fr == "ja":
         pr4_bro = pr4-pr4*0.07

        else:  
         pr4_bro = pr4-pr4*0.16    

        re = input("Rechnung berechnen? ")

        if re == "ja":
         print(("warenkorb: ") + str(list_P))
         print(("preis(netto): ") + str(pr + pr2 + pr3 + pr4))
         print(("preis(brutto): ") + str(pr_bro + pr2_bro + pr3_bro + pr4_bro))

        else:
         P = input("podukt eingeben : ")
         r5 = input("Preis: ")
         pr5 = float(r5)
         fr = input("Ist ihr Produkt Lebensmittel('ja' eingeben) oder Essen(irgendwas eingeben) ? ")
         list_P.insert(4, P)

         if fr == "ja":
          pr5_bro = pr5-pr5*0.07

         else:  
          pr5_bro = pr5-pr5*0.16    

         re = input("Rechnung berechnen? ")

         if re == "ja":
          print(("warenkorb: ") + str(list_P))
          print(("preis(netto): ") + str(pr + pr2 + pr3 + pr4 + pr5))
          print(("preis(brutto): ") + str(pr_bro + pr2_bro + pr3_bro + pr4_bro + pr5_bro))

         else:
          print("mehr als 5 produkte sind nicht erlaubt")

