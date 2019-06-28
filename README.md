# Test-provalab15

## ControlloChiuse

Chiuse 1 
Per  aumentare  la  sicurezza  nei  canali  navigabili  si  è  reso  necessario  rivedere  la  gestione  del 
sistema  di  controllo  delle  chiuse,  automatizzando  le  procedure  di  apertura  e  chiusura  e 
introducendo  la  possibilità  di  una  supervisione  remota  degli  impianti.  

In  particolare,  è  stata rivista  e  ridefinita  l’interazione  tra  il  sistema  di  controllo  delle  **chiuse**  e  le  **imbarcazioni**  in transito.

Una  chiusa  permette  alle  imbarcazioni  in  transito  in  un  canale  di  superare  un  dislivello.  La 
chiusa è formata da una **vasca** e da due **paratie** (a **monte** e a **valle**). Un’imbarcazione entra 
nella vasca e, sfruttando il principio dei vasi comunicanti, viene portata al livello desiderato. 

Il riempimento della vasca, nel caso di spostamento dal lato a valle a quello a monte del canale, 
avviene mediante l’apertura di una **valvola di afflusso**. 

Analogamente, lo svuotamento della vasca, nel caso di spostamento dal lato a monte a quello a valle, avviene mediante l’apertura di una **valvola di deflusso**. Si noti che non è necessario l’uso di pompe, in quanto sia l’afflusso sia  il  deflusso  avvengono  naturalmente.  

Prima  di  entrare  nella  vasca,  il  conducente dell’imbarcazione proveniente dal lato a valle deve prenotarne l’uso, mediante la pressione di un  pulsante  di  prenotazione  a  valle  posto  prima  delle  paratie  e  davanti  al  lato  destro dell’imbarcazione. 

Se la vasca è libera, il semaforo a valle passa dal rosso al verde. Viene quindi aperta la paratia di valle (se chiusa) per consentire all’imbarcazione di entrare nella vasca. 

Una volta nella vasca, il conducente dell’imbarcazione deve premere il pulsante di chiusura a valle, 
che attiverà la chiusura delle paratie, farà passare dal verde al rosso il semaforo a valle, attiverà 
il riempimento della vasca e l’apertura delle paratie a monte. 

Dopo essere uscito dalla vasca, il conducente dell’imbarcazione preme il pulsante di uscita a monte, per segnalare al sistema di controllo  il  transito  avvenuto.  

Analogamente,  un’imbarcazione  proveniente  dal  lato  a  monte incontrerà, nell’ordine, il pulsante di prenotazione a monte, il pulsante di chiusura a monte e il pulsante  di  uscita  a  valle,  mentre  lo  stato  di  prenotazione  è  rappresentato  dal  semaforo  a monte.  Un  sensore  di  livello  rileva  il  **livello**  dell’acqua  all’interno  della  vasca.  

Il  sistema  di controllo della chiusa gestisce l’apertura e la chiusura delle paratie, l’apertura e la chiusura delle **valvole**, l’accensione delle luci dei **semafori**, il rilevamento della pressione dei pulsanti. 

Tutte le  informazioni  relativi  agli  eventi,  ai  valori  rilevati  dai  sensori  e  ai  comandi  inviati  alle 
apparecchiature di attuazione sono registrate in un log. 

Chiuse 2 

In  seguito  a  una  variazione  delle  modalità  di  gestione  del  sistema  delle  **chiuse**  è  stato 
introdotto  il  pagamento  del  **pedaggio**.  

Ciò  ha  comportato  la  revisione  della  procedura  di apertura e chiusura e la modifica degli impianti con l’eliminazione dei due pulsanti di chiusura (a valle e a monte) e l’introduzione di un **apparecchio flottante** (posizionato su un lato della vasca)  per  la  riscossione  del  pedaggio  con  pagamento  mediante  contanti  (senza  garanzia  di resto) o apposita carta prepagata con credito a scalare. 

La procedura per l’entrata e l’uscita è modificata  solo  nella  parte  relativa  alla  pressione  del  pulsante  di  chiusura  (sostituita  con  il pagamento del pedaggio). 

In caso di mancato pagamento (per insufficiente quantità di contanti o  per  insufficiente  credito  sulla  carta  prepagata)  il  **conducente**  dell’imbarcazione  viene informato dell’evento e invitato a uscire dalla vasca premendo, entro due minuti, il pulsante di 
uscita. 

Se il pulsante di uscita non è premuto entro due minuti, viene azionata una **sirena** che 
segnala la situazione anomala e, dopo altri due minuti, il sistema si riporta nello stato di chiusa 
libera. 

L’**importo** del pedaggio varia da chiusa a chiusa. 

La sirena viene anche azionata in caso di pagamento regolare, se il conducente dell’imbarcazione non preme il pulsante di uscita entro due  minuti  dall’apertura  delle  paratie,  che  consente  il  completamento  del  passaggio  della chiusa.  

****

**Domanda n.1**. (Analisi del dominio, Chiuse 1) Dare un diagramma delle classi, considerando come classi o attributi tutti e soli i termini che nell’enunciato compaiono in grassetto. 

**Domanda n.2**. (Analisi del dominio, Chiuse 2) Dare un diagramma delle classi, considerando come classi o attributi tutti e soli i termini che nell’enunciato compaiono in grassetto. 