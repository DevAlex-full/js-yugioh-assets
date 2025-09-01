# Yu-Gi-Oh Jo-Ken-Po Edition

Um jogo interativo que combina a nostalgia do universo Yu-Gi-Oh com a simplicidade clássica do jogo Pedra, Papel e Tesoura (Jo-Ken-Po). Desafie o computador em duelos épicos usando cartas icônicas do anime!

## 🎮 Sobre o Jogo

Este projeto recria a experiência de duelo do Yu-Gi-Oh em um formato simplificado de Jo-Ken-Po, onde cada carta representa um elemento do jogo clássico:

- **Blue-Eyes White Dragon** (Papel)
- **Dark Magician** (Pedra) 
- **Exodia** (Tesoura)

## ✨ Funcionalidades

### Mecânicas de Jogo
- Sistema de duelo baseado em Jo-Ken-Po
- Interface imersiva com tema Yu-Gi-Oh
- Sistema de pontuação em tempo real
- Seleção interativa de cartas
- Campo de batalha visual para duelos

### Recursos Audiovisuais
- Vídeo de fundo temático do Yu-Gi-Oh
- Efeitos sonoros para vitória, derrota e empate
- Música de fundo ambiente (Egyptian Duel)
- Animações e efeitos hover nas cartas
- Cursores personalizados temáticos

### Interface do Usuário
- Design responsivo com elementos RPG
- Molduras douradas decorativas
- Sistema de preview de cartas
- Indicador de pontuação
- Botão de próximo duelo

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura semântica e elementos multimídia
- **CSS3**: Estilização avançada com gradientes, animações e bordas customizadas
- **JavaScript ES6+**: Lógica do jogo com async/await e manipulação DOM
- **Fontes Google**: Press Start 2P, Rubik, Secular One

## 📁 Estrutura do Projeto

```
projeto/
├── index.html
├── src/
│   ├── styles/
│   │   ├── reset.css
│   │   ├── buttons.css
│   │   ├── containers_and_frames.css
│   │   └── main.css
│   ├── scripts/
│   │   └── engine.js
│   ├── assets/
│   │   ├── icons/
│   │   │   ├── dragon.png
│   │   │   ├── magician.png
│   │   │   ├── exodia.png
│   │   │   └── card-back.png
│   │   ├── audios/
│   │   │   ├── egyptian_duel.mp3
│   │   │   ├── WIN.wav
│   │   │   ├── LOSE.wav
│   │   │   └── DRAW.wav
│   │   ├── video/
│   │   │   └── yugi.mp4
│   │   ├── cursor/
│   │   │   ├── yamiyugicursorGLOW.png
│   │   │   └── yugicursor.png
│   │   ├── rpg/
│   │   │   └── [elementos de UI RPG]
│   │   └── favicon/
│   │       └── Favicon.ico
└── README.md
```

## 🚀 Como Executar

### Pré-requisitos
- Navegador web moderno com suporte a HTML5, CSS3 e JavaScript ES6+
- Servidor web local (recomendado para evitar problemas com CORS)

### Instalação e Execução

1. **Clone ou baixe o repositório**
   ```bash
   git clone [url-do-repositorio]
   cd yugioh-jo-ken-po
   ```

2. **Execute com servidor local**
   
   **Opção 1 - Python:**
   ```bash
   # Python 3
   python -m http.server 8000
   # ou Python 2
   python -m SimpleHTTPServer 8000
   ```
   
   **Opção 2 - Node.js:**
   ```bash
   npx http-server
   ```
   
   **Opção 3 - Live Server (VS Code):**
   - Instale a extensão Live Server
   - Clique com botão direito no `index.html`
   - Selecione "Open with Live Server"

3. **Acesse no navegador**
   ```
   http://localhost:8000
   ```

## 🎯 Como Jogar

1. **Início**: O jogo carrega automaticamente com 5 cartas para você e 5 para o computador
2. **Seleção**: Passe o mouse sobre suas cartas para ver os detalhes
3. **Duelo**: Clique em uma carta para iniciar o duelo
4. **Resultado**: O resultado aparece no campo de batalha
5. **Próximo Round**: Clique no botão para continuar
6. **Pontuação**: Acompanhe seus Wins e Loses no placar

### Regras do Jogo
- **Blue-Eyes White Dragon** (Papel) vence **Dark Magician** (Pedra)
- **Dark Magician** (Pedra) vence **Exodia** (Tesoura)
- **Exodia** (Tesoura) vence **Blue-Eyes White Dragon** (Papel)

## 🎨 Características Técnicas

### Sistema de Estados
- Gerenciamento centralizado de estado do jogo
- Controle de pontuação persistente durante a sessão
- Sistema de referências DOM otimizado

### Arquitetura Modular
- Separação clara entre lógica, estilo e estrutura
- Funções assíncronas para melhor performance
- Sistema de eventos eficiente

### Design Responsivo
- Interface adaptável a diferentes tamanhos de tela
- Elementos UI escaláveis
- Suporte a dispositivos móveis

## 🎵 Recursos Multimídia

- **Vídeo de Fundo**: Atmosfera imersiva do anime
- **Áudio Ambiente**: Trilha sonora Egyptian Duel
- **Efeitos Sonoros**: Feedback audio para cada resultado
- **Cursores Customizados**: Experiência temática completa

## 🔧 Customização

### Adicionando Novas Cartas
Para adicionar novas cartas, edite o array `cardData` no arquivo `engine.js`:

```javascript
{
    id: 3,
    name: "Nome da Carta",
    type: "Tipo",
    img: `${pathImages}nova-carta.png`,
    WinOf: [array de IDs que esta carta vence],
    LoseOf: [array de IDs que esta carta perde],
}
```

### Modificando Estilos
- **Cores e temas**: Edite `main.css`
- **Botões**: Customize em `buttons.css`
- **Molduras**: Ajuste em `containers_and_frames.css`

## 🌟 Funcionalidades Destacadas

- ⚡ **Performance otimizada** com carregamento assíncrono
- 🎨 **Design imersivo** com elementos visuais detalhados
- 🔊 **Experiência audiovisual** completa
- 📱 **Responsivo** para diferentes dispositivos
- 🎮 **Gameplay intuitivo** e acessível

## 🤝 Contribuições

Contribuições são bem-vindas! Para contribuir:

1. Faça um Fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request

## 📄 Licença

Este projeto é apenas para fins educacionais e de entretenimento. Yu-Gi-Oh é uma marca registrada da Konami.

## 🎯 Próximas Funcionalidades

- [ ] Sistema de níveis de dificuldade
- [ ] Mais cartas e estratégias
- [ ] Modo multiplayer local
- [ ] Sistema de conquistas
- [ ] Estatísticas detalhadas
- [ ] Temas alternativos
