# readme  		Musteri icin sipariş girme
	
	-->menu oluşturulur 							-->superclass
	
		-müşteri(firma)//firma adı giriliyor vergiden dolayı
		-ödeme şekli		
		-kur(ödeme tipi)
		-kumaş bilgisi  ----------------------------------> db den alınacak kodlar
		-miktar
		-fiyat-------> birim fiyatı*miktar
		-sevkiyat
		-çıkış
	

	--> müşteri(firma) 
		-adı------------------------------------------->db		-->subclass
		-müşteri kodu --------------------------------->db alınacak
		-iletişim bilgileri---------------------------->db
			-telefon
			-email
			-adresler // farklı fabrikalar,farklı lokasyon
			
  	-->kumaş bilgisi-------------------------------------->db		-->subclass
		-kod
		-birim fiyatı
		-iplik çeşidi -----
		-renk
		-tipi //denim,formal....---------
	-->sevkiyat								 -->subclass
		-teslim adresi------------------------------->db
		-fatura adresi------------------------------->db
		-yurtiçi
		-yurtdışı
			-FOB //kendi ülke sınırlna teslim
			-CIF //alıcının ülke sınırında teslim
			-DAF //adrese teslim 
