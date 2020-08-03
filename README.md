
```
var elButton = document.querySelector('button');
var tempStart = new Date().getTime(); 

elButton.onclick = function() {  
  document.querySelector('#tempoFinal').innerHTML = '';
  tempStart = new Date().getTime();  
  setTimeout(Finalizar, 2000); 
}

function Finalizar() {
    var temp = (new Date().getTime() - tempStart) / 1000;
    var message = 'Tempo total: ';
    document.querySelector('#tempoFinal').innerHTML =  message + temp;
}
```
