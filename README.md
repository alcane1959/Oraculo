# Oráculo Supremo

Aplicação web humorística que gera números aleatórios, personagens fictícios, previsões astrológicas e mensagens sarcásticas personalizadas conforme o signo escolhido pelo usuário.

## Sobre o projeto

O **Oráculo Supremo | A Enciclopédia do Sarcasmo** é uma experiência interativa criada com HTML, CSS e JavaScript puro. O usuário informa quantas dezenas deseja gerar, seleciona um signo e recebe uma composição aleatória com números, nome de guru, descrição visual, horóscopo, diagnóstico cósmico, previsão financeira e outros elementos de entretenimento.

A mensagem completa é exibida na página e copiada automaticamente para a área de transferência, facilitando seu compartilhamento.

## Funcionalidades

- Geração de 1 a 100 números aleatórios entre `00` e `99`.
- Seleção entre os 12 signos do zodíaco.
- Validação da quantidade informada e do signo selecionado.
- Geração aleatória de nome e aparência para o personagem do oráculo.
- Exibição animada dos números gerados.
- Horóscopo humorístico relacionado ao signo escolhido.
- Veredito sarcástico personalizado por signo.
- Diagnóstico cósmico com indicadores aleatórios.
- Previsão financeira humorística.
- Cor da sorte, objeto de poder e animal-totem.
- Missão do dia e alerta cósmico.
- Conselho final aleatório.
- Pré-visualização da mensagem completa.
- Cópia automática do resultado para a área de transferência.
- Notificação temporária após a cópia.
- Interface responsiva com identidade visual em azul-escuro, branco e dourado.

## Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript Vanilla
- Clipboard API
- Google Fonts
  - Cinzel
  - Montserrat

## Estrutura do projeto

```text
oraculo-supremo/
├── index.html
└── README.md
```

A estrutura da página, os estilos, os vocabulários e toda a lógica de geração estão concentrados no arquivo `index.html`.

## Como executar

1. Baixe os arquivos do projeto.
2. Mantenha o `index.html` e o `README.md` na mesma pasta.
3. Abra o arquivo `index.html` em um navegador moderno.
4. Informe uma quantidade entre 1 e 100.
5. Selecione um signo.
6. Clique em **Invocar 100 Milhões de Profecias**.
7. Aguarde a exibição dos números e da mensagem completa.

Não é necessário instalar dependências, configurar banco de dados ou executar um processo de compilação.

## Como funciona

### Inicialização

Ao carregar a página, a função `gerarNomeEVisual()` seleciona aleatoriamente:

- um título para o personagem;
- um nome;
- um sobrenome humorístico;
- um cenário;
- uma roupa;
- um acessório.

### Geração dos números

A função `executarSorteio()` valida os dados informados e gera a quantidade solicitada de números entre `00` e `99`. Cada número é exibido em uma esfera com uma pequena animação de entrada.

> Os números são gerados de forma independente. Por isso, podem ocorrer repetições no mesmo resultado.

### Montagem da mensagem

Depois da geração, a função `finalizar()` combina conteúdos aleatórios dos vocabulários internos para montar uma mensagem com:

- identidade e estado visual do oráculo;
- abertura, problema e conselho;
- horóscopo e veredito do signo;
- energia espiritual e paciência;
- chance humorística de recebimento por Pix;
- diagnóstico digital;
- previsão financeira;
- elementos simbólicos de sorte;
- missão e alerta;
- números gerados;
- despedida final.

### Cópia automática

A mensagem montada é enviada à Clipboard API por meio de `navigator.clipboard.writeText()`. Após a cópia, a página exibe uma notificação durante alguns segundos.

## Personalização

Os conteúdos aleatórios estão organizados no objeto JavaScript `vocab`. É possível ampliar ou alterar as listas de:

```javascript
vocab.base
vocab.nome
vocab.sobrenome
vocab.abertura
vocab.problema
vocab.conselho
vocab.horoscopo
vocab.despedida
```

Também existem coleções específicas para cores, objetos, animais, alertas, missões, previsões financeiras, diagnósticos e descrições visuais.

As cores principais podem ser modificadas nas variáveis CSS:

```css
:root {
  --bg: #060b1a;
  --gold: #d4af37;
  --text: #1a1a1a;
}
```

## Compatibilidade

Recomenda-se utilizar um navegador moderno com suporte a:

- JavaScript;
- Clipboard API;
- animações CSS;
- `setTimeout()`;
- fontes externas do Google Fonts.

A cópia automática pode depender de permissão do navegador e funcionar melhor quando a página é aberta em um contexto seguro, como HTTPS ou ambiente local compatível.

## Limitações

- Os resultados são aleatórios e destinados apenas ao entretenimento.
- Os números podem se repetir.
- A aplicação não consulta resultados oficiais de loterias.
- O conteúdo não representa aconselhamento financeiro, espiritual ou astrológico.
- A aplicação não garante premiações, previsões ou resultados futuros.
- As fontes externas dependem de conexão com a internet.

## Uso responsável

Este projeto deve ser tratado como uma experiência humorística. Os números e textos gerados não devem ser utilizados como base para decisões financeiras, apostas ou escolhas importantes.

---

### Instalação no computador

### No Google Chrome ou Microsoft Edge:

  1. Abra o endereço publicado do projeto.
  2. Aguarde o carregamento completo da página.
  3. Clique no ícone de instalação exibido na barra de endereço ou abra o menu do navegador.
  4. Selecione Instalar aplicativo ou Instalar este site como aplicativo.
  5. Confirme a instalação.

Depois disso, o aplicativo poderá ser aberto pelo menu Iniciar, pela área de trabalho ou pelo gerenciador de aplicativos do sistema.

### Instalação no celular ou tablet

### Em navegadores compatíveis:

1. Abra o endereço do projeto.
2. Acesse o menu do navegador.
3. Selecione Instalar aplicativo ou Adicionar à tela inicial.
4. Confirme o nome e a instalação.

O ícone será adicionado à tela inicial do dispositivo.

**Observações**

A disponibilidade e o nome da opção de instalação podem variar conforme o navegador e o sistema operacional.
Abrir somente o arquivo index.html pelo computador não garante a instalação como PWA.
O projeto deve ser publicado em HTTPS para utilizar os recursos completos de instalação e service worker.
O funcionamento offline depende da configuração do service-worker.js e dos arquivos adicionados ao cache.
Atualizações no projeto podem exigir a atualização da versão do cache do service worker.

---

## Autor

**Alberto de Campos Neto**

## Aviso

> Este projeto é uma demonstração educacional desenvolvida para estudos de HTML, CSS e JavaScript. A empresa mencionada é fictícia e qualquer semelhança com empresas reais é mera coincidência.

Your site is live at https://alcane1959.github.io/Oraculo/
