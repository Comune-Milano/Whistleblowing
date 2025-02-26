# Whistleblowing

Di seguito le istruzioni necessarie per eseguire l’installazione della versione personalizzata di Globaleaks 4.11.5 su sistema Ubuntu 22.04.

I vari passaggi sono esclusivamente dedicati a chi ha in gestione il server dedicato all’applicazione.


1.	Installare globaleaks 4.11.5 eseguendo il seguente comando utilizzando il file .deb allegato alla guida:
dpkg -i globaleaks_4.11.5_all.deb
Eventualmente installare tutte le dipendenze richieste con apt.
2.	Estrarre il pacchetto pack1.tar.gz nella cartella /usr/lib/python3/dist-packages/globaleaks/
3.	Estrarre il pacchetto pack2.tar.gz nella cartella /usr/share/globaleaks/client
4.	Estrarre il pacchetto pack3.tar.gz nella cartella /var/globaleaks
5.	Riavviare il servizio globaleaks:
service globaleaks stop
service globaleaks start
6.	Verificare che il servizio sia attivo:
service globaleaks status
7.	Effettuare il login nell'applicazione tramite browser al seguente URL utilizzando le credenziali di accesso presenti nel file utenze.txt allegato alla guida:
http://127.0.0.1:8080/#/login
