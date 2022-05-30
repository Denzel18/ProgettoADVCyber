# ProgettoADVCyber
Progetto relativo al corso di  Advance Cyber Security

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/github_username/repo_name">
    <img src="images/logo.png" alt="Logo" width="250" height="80">
  </a>

<h3 align="center">Progetto di Advance Cyber Security</h3>

  <p align="center">
    <br />
    <a href="https://github.com/Denzel18/ProgettoADVCyber/Relazione.pdf"><strong>Explore the docs »</strong></a>
    <br />
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contributors">Contributors</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project
In questo elaborato l’attenzione è posta, nello specifico, sui malware che permettono di crea-
re le Botnet, cioè reti di macchine infette (bot) che poi devono essere coordinate dall’hacker
tramite un server di comando e controllo. Per contrastare un’infezione di questo tipo, spesso,
si tenta di individuare ed offuscare il server di comando e controllo; ciò, però, non è così facile
perché in risposta vengono adottate delle tecniche evasive che ne rendono difficile l’individuazio-
ne. ***Una di queste tecniche consiste nel cambiare il nome di dominio dopo un certo intervallo di
tempo, attraverso un DGA (Domain Name Generation Algorithm***

### Built With

* [Google Colab](https://colab.research.google.com/?hl=it)
* [Python 3.11](https://www.python.org/)
* [FastText](https://fasttext.cc/)
* [DGA MIXED EMBEDDING](https://gitlab.com/christian.morbidoni/dga-mixed-embeddings-ensemble/-/tree/incicco_emanuele)

<!-- GETTING STARTED -->
## Getting Started

1. Downloads Logs GARR: Selezione Logs secondo le specifiche richieste (6 gg al mese, per 12 mesi, per ogni fascia oraria, considerando solo il 10% di ciascun log) 
2. ETL: Pulizia domini sulla base della lunghezza
   1. $Lenght > 3$ e $Lenght < 100$
   2. Regex 
      ```python 
      re.match(r'.*\d*\.\d*\.\d*')
      ```
3. Divisione in n-grams 
4. Implementazione FastText e Allenamento FastText 
5. Script per Bin $\to$ Vec 
6. Implementazione Architettura Multi Input e Multi Input with Random Embeddings 


### Prerequisites
* Per lo sviluppo del progetto è richiesta l'installazione dei pacchetti relativi alla FastText, Keras, TensorFlow (per l'architettura), nlkt per la suddivisione in n_grams. Il tutto è possbile tramite il commando (il paramentro -q è relativo a ***quiet***):
  ```python
  pip install <name-package> -q 
  ```


* Per motivi si sicurezza non riportiamo informazioni relative al riperimento del dataset GARR. Possiamo solo dire che in quel caso è stato utilizzato il commando: 
  ```sh
   scp -P XXXXX studenti@XXX.XXX.XXX.XXX:/home/.../pdns_XXXX_XX_XX_XX.log.xz  /Users/name_users/Desktop
   ```

<!-- USAGE EXAMPLES -->
## Usage
Una volta scaricati i vari logs e fatto il clone del repository [DGA MIXED EMBEDDING](https://gitlab.com/christian.morbidoni/dga-mixed-embeddings-ensemble/-/tree/incicco_emanuele), sarà sufficiente eseguire lo [script](https://github.com/Denzel18/ProgettoADVCyber/Script_ADV_CYBER_NEW.ipynb)

Per ulteriori dettagli, rifarsi alla [Documentazione](https://github.com/Denzel18/ProgettoADVCyber/Relazione.pdf)



<!-- LICENSE -->
## License
Distributed under the MIT License. 

<!-- CONTACT -->
## Contributors  
Emanuele Incicco, Federico Miscia, Lorenzo Fratini, Andrea Pinciaroli, Denis Bernovschi

Project Link: [https://github.com/Denzel18/ProgettoADVCyber](https://github.com/Denzel18/ProgettoADVCyber/)


<!-- ACKNOWLEDGMENTS -->
## Acknowledgments
Progetto Sviluppato nel Corso di Advanced Cyber Security tenuto all'Università Politecnica delle Marche 

