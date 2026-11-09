# Ciclo de Estudos — edição local (V4.16)

Aplicação estática de planejamento e acompanhamento de estudos para concursos públicos.

## Publicação no Vercel

O projeto usa apenas HTML, CSS e JavaScript, reunidos em `index.html`.

1. Envie os arquivos desta pasta para a **raiz** de um repositório no GitHub.
2. No Vercel, crie um projeto e importe esse repositório.
3. Selecione **Other** em Framework Preset.
4. Deixe **Build Command** vazio (desative a etapa de build).
5. Use a raiz do projeto (`.`) como Output Directory e clique em Deploy.

Nenhum comando npm, servidor ou banco de dados é necessário nesta edição.

## Como os dados são salvos

**A aplicação continua sendo uma edição local**, mesmo quando aberta por uma URL da Vercel:
- os dados são salvos no navegador, usando `localStorage`;
- cada navegador/dispositivo mantém seus próprios registros;
- não há login nem sincronização entre dispositivos;
- ao mudar do HTML aberto no computador para a URL hospedada, os registros
  não são transferidos automaticamente.

Antes de migrar de endereço, exporte o backup JSON pela ferramenta e importe-o
ao acessar o novo endereço. Mantenha cópias do backup fora do navegador.

**Atenção:** nunca publique arquivos de backup contendo informações pessoais
no repositório. O código do site poderá ser visto por quem visitar a versão
hospedada; o conteúdo do `localStorage` dos visitantes não será enviado ao GitHub.

Esta edição não é a futura versão com autenticação e banco de dados.
