# C-digo-Limpo-RESUMO-Cap-tulos-2-4-e-5

## Nomes Significativos - 2° Capítulo 

### Use Nomes que Revelem seu Propósito

Os nomes escolhidos devem demonstrar seu propósito, ele deve dizer por que existe, o que faz e como é usado.
Por exemplo, nomes vagos como d não revelam nada, é necessário escolher nomes que especifiquem o uso e a unidade usada.
Escolher bons nomes facilitam o entendimento e a alteração do código.
Com nomes explicativos, o código fica mais explícito.


### Evite Informações Erradas

Os programadores devem evitar passar dicas falsas que confundam o sentido do código, evitando utilizar palavras cujos significados podem se desviar daquele que desejamos ou nomes muito parecidos. O uso de formatos inconsistentes para palavras leva a uma má interpretação.

Por exemplo: Letras como “l” minúsculo e “O” maiúsculo podem gerar confusão com 1 e 0.

Com uma simples troca de nome, o problema pode ser resolvido com objetividade.


### Faça Distinções Significativas

Não basta adicionar números ou palavras muito comuns, se os nomes precisam ser diferentes, então também devem ter significados distintos.
Usar números sequenciais em nomes (a1, a2) é o oposto da seleção de nomes expressivos como as palavras muito comuns que são outra forma de distinção que nada expressam.

Exemplo:         RUIM:   usuario1
                        usuario2

                 MELHOR: usuarioAdministrador
                         usuarioCliente 

 Outro exemplo:
Product, ProductInfo e ProductData não revelam nada de diferente.

O nome de uma variável jamais deve conter a palavra “variável”.

É necessário  realizar a distinção dos nomes de uma forma que o leitor compreenda as diferenças dentro do código.


### Use Nomes Pronunciáveis

Crie nomes pronunciáveis pois se não puder pronunciá-los, não terá como discutir sobre tais nomes.
A programação é uma atividade social e utilizar nomes de baixa qualidade dificultam a comunicação, pois os novos desenvolvedores do código precisarão pedir explicações quando os nomes não estão claros.

### Use Nomes Passíveis de Busca

 Nomes de uma só letra ou números não são fáceis de localizar ao longo de um texto.
Nomes longos se sobressaem aos curtos, e qualquer nome passível de busca se sobressai a uma constante no código.
 O tamanho de um nome deve ser proporcional ao tamanho do escopo.
 Se uma variável ou constante pode ser vista ou usada em vários lugares dentro do código, é imperativo atribuí-la um nome fácil para busca.

### Evite Codificações

 Codificar informações do escopo ou tipos em nomes adiciona uma tarefa extra de decifração, gerando uma sobrecarga mental desnecessária ao tentar resolver um problema. 
Nomes codificados raramente são pronunciáveis, além de ser fácil escrevê-los incorretamente.

### A Notação Húngara

 Antigamente, as linguagens de programação tinham muitas limitações. Por isso, os programadores criaram formas de colocar o tipo da variável no próprio nome

Exemplo: strNome
                 intIdade

Isso era útil porque os compiladores antigos não conseguiam verificar bem os tipos das variáveis.
Mas hoje as linguagens modernas, como Java, já fazem essa verificação automaticamente. Além disso, os editores de código ajudam a identificar erros antes mesmo de compilar.
 
 Hoje em dia, a Notação Húngara e outras formas de convenção de tipos são basicamente obstáculos.

### Prefixos de Variáveis Membro

  Você não precisa mais colocar o prefixo `m_` em variáveis membro. Para isso, suas classes e funções devem ser pequenas. E deve se utilizado um ambiente de edição que realce ou colore as variáveis membro de modo a distingui-las.
 As pessoas rapidamente aprendem a ignorar o prefixo (ou sufixo) para visualizar a parte significativa do nome.

### Interfaces e Implementações

 A melhor não enfeitar as interfaces.
O usuário não precisa saber se está usando uma interface ou não, então não é necessário colocar letras como “I” no começo (IShapeFactory). Isso só deixa o nome mais poluído.

 Exemplo: A interface ficaria apenas ShapeFactory e a implementação teria algo diferente, como ShapeFactoryImp ou CShapeFactory.


### Evite o Mapeamento Mental

 Os leitores não devem ter de traduzir mentalmente os nomes escolhidos e um nome de uma só letra é uma escolha ruim, a clareza é fundamental. Os profissionais devem escrever códigos que outros possam entender.

### Nomes de Classes

 Classes e objetos devem ter nomes com substantivo(s) Evitando palavras como Gerente, Processador, Dados ou Info no nome de uma classe.
O nome de uma classe também não deve ser um verbo.

Exemplos: Cliente, Paginawiki, Conta

### Nomes de Métodos

  Os nomes de métodos devem ter verbos, como postarPagamento ou excluirPagina.
 Métodos de acesso, alteração e autenticação devem adicionar os prefixos `get`, `set` ou `is`.
 Quando os construtores estiverem sobrecarregados, use métodos factory estáticos com nomes que descrevam os parâmetros.
 Para forçar seu uso, torne os construtores correspondentes privados.

### Não dê uma de Espertinho

  Se os nomes forem muito “espertinhos”, apenas algumas pessoas irão lembrá-los.
 Dizer o que quer expressar e expressar de forma correta o que quer dizer é fundamental. Opte por clareza no lugar de divertimento.

### Selecione uma Palavra por Conceito

Escolha uma palavra para cada ação e use a mesma em todo o projeto pois termos equivalentes usados de formas diferentes causam confusão.

Por exemplo:
Usar sempre obter()
E nunca misturar com pegar ou recuperar()

 Um léxico consistente ajuda programadores a selecionar o método correto sem busca extra.

### Não Faça Trocadilhos

Evite usar a mesma palavra para dois propósitos. Usar o mesmo termo para ideias diferentes é basicamente um trocadilho. Métodos com semânticas diferentes devem ter nomes diferentes.


### Use nomes a partir do Domínio da Solução

Use termos de Informática, nomes de algoritmos, padrões e termos matemáticos quando forem familiares aos programadores. Nomes técnicos para coisas técnicas são, geralmente, o método mais adequado.

### Use nomes de Domínios do Problema

Quando não houver uma solução “à la programador”, use nomes do domínio do problema.

 Exemplo:
em um sistema de hospital, usar nomes relacionados à medicina ou em um banco, usar termos financeiros.

Isso ajuda outros programadores a entenderem o código.


### Adicione um Contexto Significativo

Poucos nomes são significativos por si só; eles precisam de contexto. Esse contexto pode vir de classes, funções e namespaces bem nomeados. Prefixos podem ajudar, mas uma classe adequada é melhor. Variáveis isoladas podem exigir inferência do leitor, enquanto um contexto claro torna o significado evidente.     

Exemplo:
a variável state sozinha pode confundir.
mas addrState mostra que ela pertence a um endereço.

Uma solução ainda melhor seria criar uma classe Address, deixando tudo organizado.


### Não Adicione Contextos Desnecessários

Nomes curtos geralmente são melhores, contanto que sejam claros. Não adicione mais contexto a um nome do que o necessário. 




# Comentários - 4° Capítulo 


Segundo o autor, o uso adequado de comentários serve para compensar o nosso fracasso em nos expressar de forma clara através do código. Comentários mentem com frequência porque o código evolui e muda, mas os programadores raramente os atualizam. A única verdade absoluta está no próprio código.


 
### Comentarios Compensam um Código Ruim

 Muitas vezes escrevemos comentários para tentar explicar uma bagunça que nós mesmos fizemos. Em vez de gastar tempo comentando um código ruim, o correto é limpá-lo e refatorá-lo.



### Explique-se no código

 Na maioria das vezes, é perfeitamente possível expressar a intenção do programa diretamente no código. Isso pode ser resolvido simplesmente criando uma função cujo nome descreva exatamente o que se pretendia colocar em um comentário.


### Comentarios Bons

São aqueles considerados necessários ou benéficos, embora o autor ressalte que o melhor comentário é aquele que você encontrou um meio de não escrever.

### Comentários Legais

São comentários exigidos por padrões corporativos ou jurídicos logo no início do arquivo, como direitos autorais (copyright) e termos de licença. Sempre que possível, deve-se referenciar um documento externo em vez de redigir termos longos.

 
### Comentários Informativos

 Fornecem informações básicas úteis sobre a implementação, como explicar o formato esperado de uma expressão regular. No entanto, criar estruturas ou classes específicas para essas tarefas costuma ser uma solução melhor que torna o comentário supérfluo.


### Explicação da intenção 

Vão além da parte técnica e documentam a justificativa ou a motivação por trás de uma decisão de design ou de negócio tomada pelo programador.


### Esclarecimento 

Servem para traduzir o significado de parâmetros ou valores retornados que sejam obscuros ou difíceis de ler. 
É útil principalmente quando lidamos com códigos que não podemos alterar (como bibliotecas externas) , mas traz o grande risco de estar incorreto.


### Alerta Sobre Consequências

 Avisam outros desenvolvedores sobre possíveis problemas ao mexer em determinado trecho (ex: explicar por que um teste está desabilitado).


### Comentário TODO

São notas no formato `//TODO` usadas para marcar tarefas que o desenvolvedor sabe que precisam ser feitas, mas não podem ser executadas no momento. Eles servem como lembretes, mas não justificam a permanência de um código ruim no sistema.


### Destaque

 São utilizados para dar ênfase à importância de um trecho de código que, à primeira vista, pode parecer irrelevante ou supérfluo para quem lê.


### Javadocs em APIs Públicas

 Documentar adequadamente uma API que será usada publicamente é altamente benéfico e prático. Contudo, eles exigem o mesmo cuidado, pois também podem se tornar enganadores ou desonestos.


### Comentários Ruins

 A maior parte dos comentários se enquadra aqui, servindo apenas como desculpas ou suportes para códigos de baixa qualidade.

### Murmúrio

 Comentários escritos com pressa, sem atenção ou apenas para cumprir tabela. Eles acabam virando enigmas que obrigam o leitor a vasculhar outras partes do sistema para tentar decifrar o que o autor quis dizer.


### Comentários Redundantes

 Aqueles que não trazem nenhuma informação nova além do que o próprio código já deixa explícito de forma clara. Só servem para poluir visualmente e atrasar a leitura do programa.


### Comentários Enganadores

 São afirmações imprecisas ou incorretas sobre o funcionamento do código, gerando desinformação e fazendo com que outros programadores percam tempo precioso corrigindo bugs causados por falsas expectativas.


### Comentários Imperativos

 Regras rígidas e cegas que exigem que toda santa função ou variável tenha um comentário ou Javadoc. Isso resulta em amontoados de textos inúteis e confusão.


### Comentários Longos  

 Históricos de alterações deixados no topo do arquivo. Antigamente faziam sentido, mas hoje em dia são totalmente obsoletos devido aos modernos sistemas de controle de versão.


### Comentários Ruidosos 

 Comentários puramente óbvios que apenas repetem o nome da variável ou da propriedade em formato de texto estruturado, sem agregar valor algum.


### Ruídos assustadores

 Javadocs gerados automaticamente ou copiados e colados que contêm erros visíveis e mostram falta de atenção dos autores.

### Evite o comentário se é possível usar uma função ou uma variável

 Explica que, em vez de colocar um comentário explicando o que um bloco complexo faz, é preferível extrair esse bloco para uma variável ou função com um nome bem descritivo.

### Marcadores de Posição

 Linhas de comentários usadas para criar "divisões" ou seções visuais em um arquivo fonte. Devem ser evitados e usados apenas se trouxerem um benefício real evidente.


### Comentários ao lado de chaves de fechamento 

 Prática de comentar em qual bloco (como `// fim do while` ou `// fim do try`) uma chave de fechamento pertence. Se o programador sente a necessidade de fazer isso, significa que a função está longa e aninhada demais, sendo melhor reduzi-la.


### Créditos e autoria

Sistemas de controle de código fonte lembram quem adicionou o quê e quando.
Não há necessidade de poluir o código com comentários de autoria.
O sistema de controle de código fonte é um local melhor para esse tipo de informação.

### Explicação do código em comentários

Explicar o código em comentários podia ser prático no passado, mas hoje sistemas de controle de código fonte lembram o código por nós.
Não precisamos explicá-lo em comentários.
Simplesmente exclua o código.

### Comentários HTML

Códigos HTML em comentários de código fonte são uma aberração.
Dificultam a leitura dos comentários no editor/IDE.
Se forem extraídos para páginas Web, isso deveria ser responsabilidade da ferramenta, e não do programador.

### Informações não-locais

Se precisar escrever um comentário, coloque-o perto do código que ele descreve.
Não forneça informações gerais do sistema em comentários locais.
Não há garantia de que o comentário será atualizado quando o código mudar.

### Informações excessivas

Não adicione discussões históricas interessantes ou descrições irrelevantes de detalhes em comentários.
Quem lê o código não precisa dessas informações históricas.

### Conexões nada óbvias

A conexão entre comentário e código deve ser óbvia.
O comentário deve explicar o que o código não consegue explicar sozinho.
É ruim quando um comentário também precisa ser explicado.

### Cabeçalhos de funções

Funções curtas não requerem muita explicação.
Um nome bem selecionado costuma ser melhor do que um comentário no cabeçalho.

### Javadocs em códigos não-públicos

Javadocs são práticos para APIs públicas.
Em código não voltado para distribuição ao público, eles são uma maldição.
A formalidade extra dos javadocs adiciona entulho e distração.

Exemplo:
Um módulo antes considerado “bem documentado” hoje é visto como uma pequena bagunça.
O excesso de comentários e documentação pode dificultar a leitura do código.


# Formatação  - 5° Capítulo 


### O objetivo da formatação

 A formatação do código é extremamente importante para o código, ela serve como uma comunicação e essa é a primeira regra nos negócios de um desenvolvedor profissional.
A funcionalidade que você cria hoje tem grandes chances de ser modificada na próxima distribuição mas a legibilidade de seu código terá um grande efeito em todas as mudanças que serão feitas.


### Formatação vertical

Asquivos menores em Java costumam ser melhores. Ao analisar projetos como JUnit, FitNesse e Apache Tomcat, percebeu-se que muitos sistemas grandes são feitos com arquivos pequenos, geralmente com menos de 200 linhas e máximo próximo de 500. Arquivos pequenos costumam ser mais fáceis de se entender do que os grandes.


### A metáfora do jornal

Pense num artigo de jornal bem redigido. O primeiro parágrafo apresenta uma sinopse da história toda. À medida que a leitura avança, vão surgindo mais detalhes.

Desejamos que um código-fonte seja como um artigo de jornal. Os detalhes devem ir surgindo conforme se move para baixo.

Se o jornal fosse apenas uma história extensa com uma aglomeração desorganizada de fatos, datas e nomes, nós simplesmente não o leriamos.


### Espaçamento vertical entre conceitos

Cada grupo de linhas representa um pensamento completo. Esses pensamentos devem ficar separados por linhas em branco. Retirar essas linhas em branco gera um efeito notavelmente obscuro na legibilidade do código.


### Continuidade vertical

Linhas de código que estão intimamente relacionadas devem aparecer verticalmente unidas.


### Distância vertical

 Conceitos relacionados devem ficar juntos no mesmo arquivos, as funções, variáveis e métodos relacionados devem estar próximos verticalmente, isso reduz confusão e torna o código mais fácil de entender.


 As variáveis devem ser declaradas o mais perto possível do local onde serão usadas.

 Variáveis locais devem ficar no topo de cada função.

 Em loops, a variável de controle deve ficar dentro da própria estrutura do loop.

 Em raros casos pode-se declarar uma variavel no inicio de um bloco ou logo depois de um
loop em uma função razoavelmente longa. 

 Já as instâncias de variáveis  devem ficar no início da classe, porque vários métodos utilizam essas variáveis. O mais importante não é exatamente onde colocá-las, mas que estejam em um local conhecido e fácil de encontrar.


### Funções dependentes

Se uma função chama outra, elas devem ficar verticalmente próximas, a que chamar deve ficar acima da que for chamada, se possível. Isso dá um fluxo natural ao programa, facilitando encontrar as funções chamadas e aumenta consideravelmente a legibilidade de todo o módulo.

### Afinidade conceitual

 Determinados bits de código querem ficar perto de outros bits. Eles possuem uma certa afinidade conceitual e quanto maior essa afinidade, menor deve ser a distância vertical entre eles.
 Essas funções possuem uma afinidade conceitual forte, pois compartilham de uma mesma convenção de nomes e efetuam variações de uma mesma tarefa básica.

### Ordenação vertical

 De modo geral, desejamos que a função chamada fique embaixo da que a chama,  criando um fluxo natural para baixo no módulo de código-fonte, de um nível maior para um menor.
Esperamos que a maioria dos conceitos venha primeiro e os detalhes de baixo nível venham por último.


## *Formatação horizontal*

### Tamanho da linha

 A maioria dos programadores prefere linhas curtas. O antigo limite de 80 caracteres ainda serve como referência.
Hoje pode-se usar até 100 ou 120 caracteres, mas sem exageros.
Linhas muito grandes dificultam a leitura e indicam falta de cuidado na organização do código.  O ideal é escrever código limpo e fácil de visualizar sem precisar rolar horizontalmente a tela.

### Espaçamento e continuidade horizontal

 Usamos o espaço em branco horizontal para associar coisas que estão intimamente relacionadas e para desassociar outras fracamente relacionadas.

Espaços ao redor de = destacam atribuições.

Não se coloca espaço entre os nomes das funções e os parênteses de abertura. 

Espaços também ajudam a mostrar prioridade matemática:

Multiplicações geralmente ficam sem espaços (2*a) já a soma e subtração costumam usar espaços (a + b) por terem menor prioridade.

Ferramentas automáticas de formatação podem remover essas diferenças visuais importantes.

### Alinhamento horizontal

 Esse tipo de alinhamento não é prático pois ele parece enfatizar as coisas erradas afastando do propósito real.
O autor prefere declarações e atribuições não alinhadas. Se tiver listas longas que precisem ser alinhadas, o problema está no tamanho das listas, e não na falta de alinhamento.

### Endentação

 Um arquivo-fonte é mais como uma hierarquia do que algo esquematizado.
 A fim de tornar visível a hierarquia desses escopos, endentamos as linhas do código-fonte de acordo com sua posição na hierarquia. Instruções no nivel do arquivo, como a maioria das
declarações de classes, não são endentadas. Métodos dentro de uma classe são endentados um nivel à direita dela. Implementações do método são implementadas um nivel à direita da declaração do método. Implementações de blocos são implementadas um nível à direita do bloco que as contém, e assim por diante.
 Os programadores dependem bastante desse esquema de endentação, sem a endentação, os programas seriam praticamente ininteligíveis para humanos.

### Ignorando a endentação

 Às vezes, ficamos tentados a não usar a endentação em estruturas if curtas, loops while pequenos ou funções pequenas, mas isso dificulta a leitura, é preferível expandir e endentar corretamente.

### Escopos minúsculos

 De vez em quando, o corpo de uma estrutura while ou for é minúscula, sendo facil se enganar com um ; quietinho lá no final de um loop while na mesma linha. A menos que você torne esse símbolo visível endentando-o em sua própria linha, fica difícil visualizá-lo. Ter uma boa formatação ajuda encontrar bugs e entender o código rapidamente.


### Regra de equipes

 Todo programador tem suas regras de formatação preferidas, mas se ele for trabalhar em equipe, as regras tem que ser as mesmas para todos pois uma equipe de desenvolvedores deve escolher um único estilo de formatação para que o software tenha um estilo consistente.

 



 *O resumo dos capitulos 2, 4 e 5 do livro "Código Limpo", escrito por Robert Cecil Martin, é interessante para quem está iniciando na área, pois apresenta diversos conselhos úteis e destaca os principais erros cometidos por programadores. Em vários momentos, é enfatizado a diferença entre um iniciante e um verdadeiro profissional da programação, mostrando como pequenos detalhes fazem grande diferença na qualidade do código.
 Além disso, ele compartilha opiniões baseadas em códigos analisados ao longo de sua experiência, explicando maneiras diferentes, mais organizadas e mais ágeis de desenvolver software. Dessa forma, o conteúdo não ensina apenas técnicas, mas também incentiva uma visão mais profissional sobre escrita de código, legibilidade e boas práticas no desenvolvimento.
 A programação não é apenas fazer o sistema funcionar, mas também escrever códigos claros e fáceis de entender.*
