# Tutorial - Diárias e Passagens
[![By - TRF6](https://img.shields.io/static/v1?label=By&message=TRF6&color=700074&style=for-the-badge)](https://trf6.jus.br)

## Etapa 1
Faça login como editor em [http://trf6.jus.br/editores](http://trf6.jus.br/editores)

---

## Etapa 2
- Abra página de diárias e passagens **2 vezes**
- Uma (página principal) nós vamos editar, e a outra, vamos adicionar `/editor` no final da URL para acessarmos o editor
  - Página principal: [https://portal.trf6.jus.br/portal-da-transparencia/gestao-de-pessoas/diarias](https://portal.trf6.jus.br/portal-da-transparencia/gestao-de-pessoas/diarias)
  - Editor: [https://portal.trf6.jus.br/portal-da-transparencia/gestao-de-pessoas/diarias/editor](https://portal.trf6.jus.br/portal-da-transparencia/gestao-de-pessoas/diarias/editor)

**OBS:** no momento, a página está em teste, portanto, `/diarias` deve ser trocado para `/diarias-teste` em todos os links temporariamente.

---

## Etapa 3
- Na edição da página principal, vamos clicar em cima da tabela e selecionar **`Edit code`**
![Imagem representativa](https://i.imgur.com/Cck5zqS.png)
- No topo da caixa que abrir, selecione a aba **`JavaScript`**
![Imagem representativa](https://i.imgur.com/xjkqG52.png)
- Selecione tudo que estiver dentro da caixa de texto (`Ctrl + A`) e copie (`Ctrl + C`)
  - Você também pode fazer isso clicando em cima com o botão direito, sendo possível selecionar tudo e copiar
![Imagem representativa](https://i.imgur.com/ReCqjjT.png)

---

## Etapa 4
- No editor, aberto na segunda página, vamos clicar em **`Colar JSON`**
![Imagem representativa](https://i.imgur.com/Vxn0NCx.png)
- Ao abrir uma caixa, no campo de texto, vamos colar (`Ctrl + V`) o que tínhamos copiado
  - É possível colar clicando com o botão direito em cima do campo também
- Ao colar, clique em **`Carregar`** para atualizar o editor
![Imagem representativa](https://i.imgur.com/hD4VBMY.png)
- E pronto, o editor vai estar preenchido com a versão atual dos dados da tabela, pronto para você poder fazer as alterações
![Imagem representativa](https://i.imgur.com/ZmZtbcJ.png)

---

## Etapa 5
O editor foi feito o mais intuitivo possível, então tudo está fácil de entender.
- Para adicionar um novo mês, clique em **`Adicionar Mês`**
- Para editar ou excluir um mês, clique em **`Editar`**/**`Excluir`** ao lado do mês desejado
![Imagem representativa](https://i.imgur.com/hgSbn7u.png)

Aqui vamos mostrar como adicionar um novo mês, mas o processo de edição é semelhante

---

## Etapa 6 - adicionando um novo mês

### 1) Enviando o(s) arquivo(s) para as mídias do WordPress
- No [painel de admin](https://portal.trf6.jus.br/wp-admin/) acesse a [Biblioteca de mídia](https://portal.trf6.jus.br/wp-admin/upload.php) do WordPress
![Imagem representativa](https://i.imgur.com/Z2IBMpc.png)
- No seu computador, abra a pasta onde o arquivo que você deseja inserir na tabela está
- Arraste o arquivo da pasta para a página da biblioteca de mídia
![Imagem representativa](https://i.imgur.com/2CYTZus.png)
- Feito o envio, note que ele possivelmente será o primeiro arquivo a aparecer. Clique nele!
![Imagem representativa](https://i.imgur.com/HH6KiNK.png)
(Ignore o detalhe de que na print abaixo só aparece ele. No seu, procure pelo arquivo com o mesmo nome que você colocou)
- Na caixa que aparecer, no canto direito, tem um botão azul para copiar a URL. Clique nele para copiar a URL do arquivo.
![Imagem representativa](https://i.imgur.com/q4FJ54N.png)

E pronto, você tem a URL do arquivo preparado para ser colado no editor. Agora vamos criar o mês e adicionar o arquivo na tabela!

### 2) Criando mês na tabela
- Vá para o editor e, no topo, escolha em qual adicionar: TRF6 ou SJMG
- Clique no botão **`Adicionar Mês`**
- Na caixa que aparecer, vamos digitar o ano e selecionar o mês que queremos adicionar na tabela
  - Não adicione um mês mais de uma vez. Nesses casos, edite o mês já existente
- Para adicionar uma diária, clique em **`Adicionar Diária`**
  - Em `Label`, preencha com o nome do mês todo em maiúsculo seguido do formato do arquivo. Ex: `FEVEREIRO.PDF`
  - Em `URL`, cole a URL do arquivo que copiamos na biblioteca de mídias
- Para adicionar uma passagem, faremos o mesmo, porém clicando desta vez em **`Adicionar Passagem`**
  - Note que nela temos um campo novo, que é o `Tipo`. 
  - Para adicionar um arquivo, escolha `Link`, e para adicionar um texto informativo no lugar, escolha `Texto`
  - No caso de link, os campos são semelhantes. No caso de texto, apenas insira o texto desejado na caixa que aparecer
- Por fim, clique em **`Salvar Mês`** lá em baixo para concluir a adição do mês

![Imagem representativa](https://i.imgur.com/9vISaNY.png)

---

**Agora vamos fazer o processo inverso do que fizemos lá no início, a fim de pegar as mudanças e passar para o WordPress.**

## Etapa 7
- Terminada a edição de tudo, clique em **`Copiar JSON`**
![Imagem representativa](https://i.imgur.com/xFM3CVc.png)
- Na caixa que aparecer, clique em **`Copiar para Área de Transferência`** lá em baixo
![Imagem representativa](https://i.imgur.com/Wd5C1io.png)

## Etapa 8
- Na edição da página principal, **se a caixa de edição já não estiver aberta**, vamos clicar em cima da tabela e selecionar **`Edit code`**, e depois, selecionar a aba **`JavaScript`**
![Imagem representativa](https://i.imgur.com/Cck5zqS.png)
![Imagem representativa](https://i.imgur.com/xjkqG52.png)
- Selecione tudo que estiver dentro da caixa de texto (`Ctrl + A`) e cole o que copiamos no editor (`Ctrl + V`)
  - Você também pode fazer isso clicando em cima com o botão direito, sendo possível selecionar tudo e colar
![Imagem representativa](https://i.imgur.com/dNecjVS.png)
- Feito isso, clique em **`Update`** lá em baixo
![Imagem representativa](https://i.imgur.com/rB2dS6O.png)
- E salve as alterações feitas na página lá em cima em **`Save`**
![Imagem representativa](https://i.imgur.com/8lNvSz8.png)