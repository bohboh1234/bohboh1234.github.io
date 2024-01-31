# bohboh1234.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tempo Insieme</title>
    <style>
        body {
            text-align: center;
            padding: 50px;
            font-family: Arial, sans-serif;
        }
        p {
            font-size: 18px;
            margin: 10px;
        }
    </style>
</head>
<body>

    <h1>Stiamo insieme da</h1>
    <p id="tempoInsieme"></p>

    <div>
        <p>Mi stavo annoiando, quindi ho deciso di creare questo sito.</p>
        <p>Stiamo insieme dal 28 dicembre 2023 (anche se in realtà è successo ai primi di gennaio).</p>
        <p>Non dimenticarti mai che questa data è la somma di:</p>
        <ul>
            <li>Il nostro primo incontro, 24 settembre</li>
            <li>Il nostro primo bacio, 4 ottobre</li>
            <li>La nostra prima volta blbl, il 22 ottobre</li>
            <li>Mi hai chiesto di metterci insieme il 5 gennaio</li>
            <li>E siamo andati a mare il 9 quindi sì, fa 28.</li>
        </ul>
        <p>Ricordo ancora quando quel giorno chiudemmo, più per scelta tua che mia, però vabb. Mi ricordo ancora che cercavo di convincere me stessa che era la cosa giusta e che avevamo sbagliato ad iniziare tutto quello.</p>
        <p>Col passare dei giorni quel pensiero è diventato ‘vabbè se è destino ci rincontreremo, se è destino, si farà risentire’.</p>
        <p>Non dimenticherò mai neanche quando avevo appena finito danza e mi ritrovai il tuo nome tra le notifiche e per un attimo non riuscivo a capire, poi aprii il messaggio con la tua foto vestito da kiwi e già in quell’istante realizzai quanto mi era mancata la tua presenza.</p>
        <p>Ma ovviamente non parlo di presenza fisica, parlo di una tua foto, un tuo messaggio, quando, fino al giorno prima, l’unico modo che avevo per sentirmi ancora in qualche modo legata a te era mettere i tik tok con le canzoni che ascoltavamo in macchina, con la speranza che l’avresti ascoltato.</p>
        <p>Da lì è stato tutto un crescendo di emozioni, belle e brutte, un po’ perché mi mancavi, un po’ perché amavo sempre di più parlare con te; e ora siamo qui che ogni tanto ti scrivo questo tipo di messaggi perché in qualche modo mi fanno sentire più vicina a te.</p>
        <p>Spero davvero che le cose fra di noi vadano sempre bene e anche se a volte mi arrabbio ricordati sempre che ti amo tantissimissimo e ti prometto che per qualunque cosa ci sarò. Miraccomando leggi questo messaggio ogni volta che ti manco e ti senti un po giù, magari anche a te fanno l’effetto di sentirmi più vicina❣️</p>
    </div>

    <script>
        // Data di inizio
        const dataInizio = new Date('2023-12-28T00:00:00');
        
        function calcolaTempoInsieme() {
            const dataCorrente = new Date();
            const differenza = dataCorrente - dataInizio;
            
            const millisecondiInSecondo = 1000;
            const millisecondiInMinuto = millisecondiInSecondo * 60;
            const millisecondiInOra = millisecondiInMinuto * 60;
            const millisecondiInGiorno = millisecondiInOra * 24;

            const giorni = Math.floor(differenza / millisecondiInGiorno);
            const ore = Math.floor((differenza % millisecondiInGiorno) / millisecondiInOra);
            const minuti = Math.floor((differenza % millisecondiInOra) / millisecondiInMinuto);
            const secondi = Math.floor((differenza % millisecondiInMinuto) / millisecondiInSecondo);

            document.getElementById('tempoInsieme').textContent = `${giorni} giorni, ${ore} ore, ${minuti} minuti, ${secondi} secondi`;
        }

        // Calcola il tempo insieme all'avvio
        calcolaTempoInsieme();

        // Aggiorna ogni secondo
        setInterval(calcolaTempoInsieme, 1000);
    </script>
</body>
</html>
