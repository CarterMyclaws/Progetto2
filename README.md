# Progetto2
Created with CodeSandbox

Questo sito rappresenta una collezione di tutti i personaggi e gli episodi della serie TV "Rick and Morty". La serie racconta di una famiglia in cui Rick Sanchez, nonno di Morty Smith e genio intergalattico con la risposta sempre pronta, ha la capacità di viaggiare attraverso lo spazio e il tempo, solo che invece di usare questo "potere" per fare del bene, lo usa invece per divertirsi e fare nient'altro che il suo interesse. Rick si porta sempre appresso suo nipote Morty in ogni avventura e insieme combinano disastri. 

Il sito si apre sulla pagina di Login che permette di inserire il proprio username registrandolo nello storage localhost e successivamente sul DB Firebase una volta inserito un personaggio preferito. Dalla Dashboard si possono accedere a due sezioni: "Characters" ed "Episodes".

La sezione "Characters" presenta due viste dei contenuti: vista cards o vista lista (triggerabili con il tasto a destra di fianco al tasto "cerca"). Il tasto cerca è provvisto di autocomplete e rimanda direttamente alla scheda del personaggio selezionato.
Nella scheda "Characters" sono presenti delle cards con tutti i personaggi che vengono caricati dinamicamente dall'API e provvisti dell'icona "preferito" già selezionata o meno in base ai risultati della chiamata al DB. È possibile visitare ogni personaggio tramite l'apposito tasto "Esplora" o aggiungerlo ai preferiti cliccando sull'icona del cuore. Se si seleziona "Esplora", viene caricata una pagina con ulteriori informazioni sul personaggio, compresa una sezione in cui vengono indicati, se presenti, gli episodi in cui compare.

Da qui, o dalla toolbar/drawer, si può procedere alla sezione "Episodes" che incorpora delle cards, una per ogni stagione, con all'interno le liste degli episodi appartenenti alla relativa stagione. Selezionando un episodio viene caricata la pagina relativa con la descrizione (purtroppo solo un esempio perché non mi è stato possibile integrare l'API di Wikipedia come avevo inizialmente progettato), ed una sezione con i personaggi presenti in quell'episodio.

Infine, è presente una sezione clicccando in alto a destra sull'icona dello user, che presenta la possibilità di fare il logout oppure la possibilità di vedere i propri personaggi preferiti.
