#Upustvo za koristenje git-a kroz cmd ili terminal

1. Sa git clone komandom smijestamo fajlove iz skladista repo u foldera hello-world,a mozemo specificirati i ime foldera ako zelimo
2. Sa komandom git rm -rf brisemo helo-world folder
3. Sa komandom git config --global user.name "" setiramo ime tako da se zna ko je mjenjao code i sta je radio --global flag oznacava da cemo jednom ovo setirati i da ce se te postavke sacuvati npr. user.name "Goran Radmanovic"
4. Sa komandom git config --global user.email setiramo email tako da se zna ko je mjenjao code i sta je radio --global flag oznacava da cemo jednom ovo setirati i da ce se te postavke sacuvati npr. user.name "goranradmanovic@gmail.com".A sa komandom git config user.name ili user.email provjeravamo da li je sve dobro setirano 
5. Sa komandom u cmd-u ili terminalu na Linuxu git status mozemo vidjeti nasu granu 'branch' i koje grane imamo 'origin/master' je glavna grana
6. Sa komandom touch i imenom fajla sa ekstenzijom stvaramo taj fajl u folderu npr. tocuh index.html u linuxu
7. Sa komandom git add ododjemu fajl u pracenje,sa zvjdicom dodjemo sve fajlove,a mozemo napisati i ime foldera

#commited znaci da ce se sve promjene koje smo napravili snimiti,mozemo napraviti commiteda koliko hocemo prije nego sto uplodujemo na server
#commited se koristi da bi mogli pratiti promjene na fajlovima koje smo modifikoval. Poslije svakog commita moramo te promjene snimiti,a to radimo
#sa komandom git add pa ime fajla ili *

8. Commiting se vrsi pomocu komande git commit -m '-m oznacava da dajemo commitu poruku' poruka mora biti deskriptivna da bi dr. koji rade na projektu mogli shvatiti o cemu se rad
9. Sa komandom git log mozemo vidjeti sve promjene koje smo napravili na fajlovima,a mozemo napisati i git log --pretty=oneline da bi nam svi logovi bili na jednoj liniji i pregledniji, ili git log --pretty=oneline -2 da nam prikaze dvije log poruke
10. Da bi ove promjene snimili u skladiste tj. repository moramo koristiti komandu git push origin master, koja je nasa glavna grana
11. Sa komandom git pull povlacimo sve izmjene sa GitHub-a na nase lokalne fajlove na kop.,ako je neko npr. mijenjao nase fajlove na GitHub-u ili sl.

#Braching je proces kreiranja novog pointera koji nam omogucava da radimo na istom codu ali u sigurnom okruzenju gdje mozemo raditi sta zelimo i odbaciti promjene koje ne zelimo,a ako smo zadovoljni mozemo ovu granu spojiti sa dr. granom

12. Da bi napravili granu koristimo komandu giti branch hello-england,'hello-england je ime grane',a sa opcijom -b automatski nas prebacuje na novu granu
13. Sa komandom git checkout hello-england se prebacujemo manuelno na tu granu
14. Sa komandom git branch merge hello-england spajamo ovu granu sa master granom
15. Sa komandom git branch -d hello-england brisemo ovu granu
16. Sa komandom git push origin --delete hello-england brisemo granu sa GitHub stranice
17. Za fajlove koje ne zelimo ucitiati na GitHub npr. koji sadrze sifre od baze podataka ili od javnih API napravimo .gitignore fajl u nasem folderu u kome radimo i u njemu upisemo fajl koji zelimo da izostavimo. Poslije toga napravimo dodavanje tog fajla sa git add *,i onda git commit -m "" sa porukom,i na kraju git push da ucitamo na GitHub
18. Sa komandom git help gitignore fajl dobijamo sve opcije koje imamoza rad sa gitignore fajlom
