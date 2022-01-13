#!/bin/sh

function dosyaSikistir(){

FILE=`zenity --file-selection --title="Sıkıştırılacak Dosyayı Seçiniz."`

case $? in 
0) 
	tar -cvzf $FILE.tar.gz $FILE;;
1) 
	echo "Hiçbir dosya seçilmedi.";; 
-1) 
	echo "Hiçbir dosya seçilmedi.";; 
esac

zenity --info --no-wrap --text="$FILE sıkıştırıldı."
}

function dosyaAc(){

FILE=`zenity --file-selection --title="Ayıklanacak Dosyayı Seçiniz."`

case $? in 
0) 
	tar -xvf $FILE -C /home/$USER/Documents;;
1) 
	echo "Hiçbir dosya seçilmedi.";; 
-1) 
	echo "Hiçbir dosya seçilmedi.";; 
esac

zenity --info --no-wrap --text="$FILE ayıklandı."

}

ans= zenity  --question \
        --title="Dosya Sıkıştırma/ Ayıklama" \
        --text="Dosyaya Yapılacak İşlemi Seçiniz" \
        --width=350 \
        --height=150 \
        --ok-label Sıkıştır\
        --cancel-label="Ayıkla"


case $? in
0)
	dosyaSikistir;;
1)
	dosyaAc;;
esac
	



