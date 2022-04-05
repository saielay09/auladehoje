# Projeto loteca
Este é um projeto de simulador de loteria, onde o usuário digita 6 numeros e realiza o sorteio de outros 6 números.
No final é verificado quantos acertos o usuário obteve.

## Tecnologias utilizadas
- **HTML**: estrutura do site
- _CSS_: estilização do site
- *_JS_*: Funções do site
- ~~BootStrap~~: Não foi utilizado

### Melhorias possíveis
 1. [ ] Subir para GitHubPages_
 2. [ ] Alterar os alerts_
 3. [ ] Utilizar o BootStrap_
 4. [ ] Deixar responsivo_
 
 ### disponibilizado em
 [GitHubPages](https://saielay09.github.io/lotecaci/)
 
 ### Prints da tela
 
| ID | Primeira Tela | Segunda Tela |
|----|---------------|----------------|
| 1 | Loteca Limpa| Loteca preenchida |
| 2 | ![Capturar3](https://user-images.githubusercontent.com/101192829/161783009-161f7702-dd7b-4229-8921-4d048f4826d1.PNG)|![image](https://user-images.githubusercontent.com/101192829/161782687-4b9a9df4-f39f-4ca2-8ed0-a1c6ec9497fe.png)

### Função principal
```
function sorteio (){
    if(numEsco.length == 6){
        var cont = 0;
        numSort=[]
        while(cont < 6){
            let num = Math.random() * 60
            num = Math.ceil(num);
            if(!numSort.includes(num)){
                numSort[cont] = num;
                console.log(numSort)
                cont++
            }
       
        } 
    document.getElementById("sorteados").innerHTML = numSort;
    contAcertos();
    }else{
        alert("É necessário digitar os seis numeros antes de sortear")
    }
    
}
```
### Para comando git
para iniciar o projeto
``` bash:
git init
```


