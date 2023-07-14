# buyuk-harfe-cevirme
Python ile metin içindeki elemanların çifte indekse sahip olan küçük harfleri büyük harfe çevirme

"""mecbure""" 
""" soru : indexi çift olanları büyük yaz tek olanları küçük yaz"""

def alternating(string):
    new_string=" " #boş küme yapıyoruz çünkü yeni gelen durumu kaydediyoruz.
    # girilen string'in index'lerinde gez.
    for string_index in range(len(string)):
        #index çift ise büyük harfe çevir.
        if string_index % 2 ==0:
            new_string += string[string_index].upper()
        #index tek ise küçük harfe çevir.    
        else:
            new_string += string[string_index].lower()
    print(new_string)
alternating("mecbure")  
