// Inizializziamo le variabili per le medie mobili
var ma21 = sma(close, 21);
var ma55 = sma(close, 55);

// Controlliamo se le medie mobili si incrociano
if (crosses(ma21, ma55))
{
    // Se la media mobile 21 attraversa quella a 55 dall'alto verso il basso, generiamo un segnale di vendita
    if (ma21[1] > ma55[1] && ma21[0] < ma55[0])
    {
        // Inseriamo qui il codice per generare il segnale di vendita
    }
    // Altrimenti, se la media mobile 21 attraversa quella a 55 dal basso verso l'alto, generiamo un segnale di acquisto
    else if (ma21[1] < ma55[1] && ma21[0] > ma55[0])
    {
        // Inseriamo qui il codice per generare il segnale di acquisto
    }
}
