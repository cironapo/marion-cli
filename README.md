# marion-cli
Creazione di un nuovo progetto marion
```bash
marion init nome_progetto
```
Per clonare un progetto esistente 
```bash
marion clone url_repository
```
Avvio ambiente di sviluppo
```bash
marion up [[-d]]
```
Shutdown del progetto
```bash
marion down
```
## Database  
In fase di sviluppo **Marion** utilizza una cartella nella root del progetto denominata **mysql** in cui viene memorizzato il database in maniera persistente.  
Nella fase di installazione del progetto la cartella viene popolata con il database di base di Marion.  
E' possibile interagire con il databse attraverso la cli mediante i seguenti comandi.  

**Aggiornamento database**  
Il seguente comando permette di effettuare un aggiornamento del database locale con quello presente nella root del progetto nel file **database.sql**
```bash
marion db refresh
```
**Esportazione database**   
Il seguente comando permette di esportare il database corrente. Il file viene esportato nella root del progetto con il nome **database.sql**
```bash
marion db export
```
## Moduli 
**Creazione modulo**  
Il seguente comando permette di creare un modulo per marion
```bash
marion module create nome_modulo
```
**Lista moduli**  
Il seguente modulo permette di visualizzare la lista dei moduli presenti nel progetto. E' possibile fare anche un filtro per nome del modulo utilizzando l'opzione **--like=key_search**
```bash
marion module list [[--like=key_search]]
```