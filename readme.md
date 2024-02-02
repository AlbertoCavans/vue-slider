# VUE SLIDER

## Obiettivo

- Partendo dal markup della versione svolta in js plain, rifare lo slider ma questa volta usando Vue.
- Bonus:
  1. al click su una thumb, visualizzare in grande l'immagine corrispondente
  2. applicare l'autoplay allo slider: ogni 3 secondi, cambia immagine automaticamente
  3. quando il mouse va in hover sullo slider, bloccare l'autoplay e farlo riprendere quando esce

## Procedimento

- Impostare il collegamento fra main.js e index.html con la struttura di base (il collegamento fra index.html verso main.js è già fornito)
- Mettere l'array di slides dentro al return della struttura di base
- Con v-bind:src impostare l'immagine del DOM perché possa cambiare assieme alla varibile corrispettiva scelta sul main.js
- Creare i collegamenti in doppia graffa su index.html per far cambiare anche titolo e testo delle slides
- Con v-for e v-bind impostare le slides della sidebar perché scorrano col cambiare dell'idex dell'array presente su main.js
- Impostare @click="function()" per impostare il cambio slide con arrow next e arrow prev
- Usare @click per cambiare immagine anche cliccando sulle slides presenti nella sidebar
- Usare setIterval per impostare lo scorrimento automatico
- Usare clearIterval per bloccare lo scorrimento automatico in caso di @mouseover (che si disattiva in caso di @mouseleave)
