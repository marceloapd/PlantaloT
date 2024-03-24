# Planta-IoT

<!---Esses são exemplos. Veja https://shields.io para outras pessoas ou para personalizar este conjunto de escudos. Você pode querer incluir dependências, status do projeto e informações de licença aqui--->

![GitHub repo size](https://img.shields.io/github/repo-size/marceloapd/planta-iot?style=for-the-badge)
![GitHub language count](https://img.shields.io/github/languages/count/marceloapd/planta-iot?style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/marceloapd/planta-iot?style=for-the-badge)

<img src="https://user-images.githubusercontent.com/71731452/135922766-871c97f0-67c5-46b8-b972-76a32027aeaa.png" alt="exemplo imagem">


> Trata-se de uma API ligada a uma planta que avisa quando precisa de agua.

### Ajustes e melhorias

O projeto ainda está em desenvolvimento e as próximas atualizações serão voltadas nas seguintes tarefas:

- [x] Tweetar frases relacionadas a plantas todas as manhãs.
- [x] Piscar led a cada request
- [ ] Corrigir erro intermitente de não salvar senha WiFi
- [ ] Feature para agradecer quando é irrigada
- [ ] Painel de controle no front-end
- [ ] Regressão linear para fazer previsões de quando regar a planta novamente.

## 💻 Pré-requisitos

Antes de começar, verifique se você atendeu aos seguintes requisitos:
<!---Estes são apenas requisitos de exemplo. Adicionar, duplicar ou remover conforme necessário--->
* Você possui `ESP8266 e um Sensor de Umidade do Solo`
* Você instalou a versão mais recente de `Node.js / VSCode / Driver CH340`
* Você tem uma máquina `Windows / Linux / Mac`.

## 🚀 Instalando Planta-IoT

Para instalar o Planta-IoT, siga estas etapas:
 
Monte o circuito abaixo:
  
<img src="https://user-images.githubusercontent.com/71731452/135925449-a17d6983-8189-41a3-a064-a661ccfdb9e1.png" width="812" height="357" alt="esquematico">
 
Abra a pasta firmware utilizando a extensão [PlatformIO](https://platformio.org/install/ide?install=vscode) do VSCode e faça upload do firmware.
 
![ezgif com-gif-maker](https://user-images.githubusercontent.com/71731452/135932280-bd088aac-62ac-4487-b974-5555657336fd.gif)

Agora dentro da pasta twitterAPI execute os comandos:

```
npm install
```

## ☕ Usando Planta-IoT

Para usar Planta-IoT, siga estas etapas:

Com o ESP8266 ligado conecte a rede WiFi de nome "Planta IoT" e informe as credenciais
 
<img src="https://user-images.githubusercontent.com/71731452/135929703-6bf5a1d3-43ae-4a34-a354-234f56ded094.jpg" width="270" height="377" alt="WiFi">  |  <img src="https://user-images.githubusercontent.com/71731452/135929409-0cc3ed30-5943-4edc-b937-78b8c19495e1.jpg" width="270" height="377" alt="WiFi"> |  <img src="https://user-images.githubusercontent.com/71731452/135929922-74966263-9418-4a75-836b-fc6827523bf1.jpg" width="270" height="377" alt="WiFi"> 
 
Dentro da pasta twitterAPI rode o comando:
```
node main.js
```
<!-- ![ezgif com-gif-maker (2)](https://user-images.githubusercontent.com/71731452/135933836-e5c2c3bf-a0d0-42f4-85b0-dd1362df51f3.gif) -->
Quando a planta Tweeta ?

Todo dia as 08:00 A.M a "planta" ira tweetar uma frase com sua umidade do solo atual:

<img src="https://user-images.githubusercontent.com/71731452/135941176-1f31361b-67e9-4a99-835a-384a73ef65c0.gif" width="411" height="373" alt="exemplo de funcionamento"> | <img src="https://user-images.githubusercontent.com/71731452/135941187-3f9dbaed-2b0f-4674-9334-85c72cdd4c5b.gif"  width="411" height="373" alt="exemplo de funcionamento">

Caso a planta receba muito agua a mesma ira tweetar um aviso.

Caso a planta perca a conexão com seu sensores ou a API a mesma ira tweetar um aviso.

## 🤝 Colaboradores

Agradecemos às seguintes pessoas que contribuíram para este projeto:

<table>
  <tr>
    <td align="center">
      <a href="#">
        <img src="https://avatars.githubusercontent.com/u/71731452?v=4" width="100px;" alt="Foto do Marcelo Assis no GitHub"/><br>
        <sub>
          <b>Marcelo Assis</b>
        </sub>
      </a>
    </td>
  </tr>
</table>

## 📝 Licença

Esse projeto está sob licença. Veja o arquivo [LICENÇA](LICENSE.md) para mais detalhes.

[⬆ Voltar ao topo](README.md)<br>
