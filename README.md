# PLANO ESTUDOS PROGRAMAÇÃO

Presente plano de estudos foi desenvolvido através do *RoadMap* https://roadmap.sh/backend. 

# Internet

## Como funciona a internet?

## O que é HTTP?

## Como funcionam os navegadores?

## O que é DNS e como funciona?

## O que é Domain Name?

## O que é hospedagem?

## Conhecimento básico de front-end

### HTML

### CSS

### JAVASCRIPT

# Sistemas Operacioanis e Conhecimentos em geral 

## *Threads* e *Concurrency*

## Gerenciamento de processos

## Gerenciamento de memória

## Comunicação entre processos

## Gerenciamento de E/S

## Noções básicas de POSIX

## Conceitos básicos de rede

## Uso do terminal e Comandos Básicos

# Linguagem programação

## Java

# Clean Code

## Regras gerais

### Siga as convenções
> Se você começou agora em um projeto ou acabaram de definir suas convenções, siga-as! Se utilizam por exemplo constantes em maiúsculo, enumeradores com E como prefixo, não importa! Siga sempre os padrões do projeto.

### KISS
> Mantenha as coisas simples! Então, Keep It Stupid Simple (Mantenha isto estupidamente simples - KISS)!

### Regra do escoteiro
> "Deixe sempre o acamapamento mais limpo do que você encontrou!" O mesmo vale para nosso código. Devolva (Check in) sempre o código melhor do que você o obteve.

### Regras de design
> Mantenha dados de configuração em alto nível.Evite sobrescrever configurações em métodos dentro de Controllers ou algo do tipo.

### Polimorfismo no lugar de IFs
>Um IF ou condicional, como o nome diz, traz uma tomada de decisão a nossa aplicação, o que implica no aumento da complexidade da mesma. No geral devemos evitar o uso excessivo destes.
Nestes cenários, opte sempre pelo polimorfismo ao invés de tomar decisão em todo método que cria.

### Mult-thread
> Sempre que necessário utilize processamento em Threads separadas.

### Evite configurações desnecessárias
> Evite deixar configurações no sistema só por que alguém ainda não definiu como aquilo deve ser. Isto polui o código e traz uma complexidade desnecessária.

### Utilize injeção de dependência
> Sempre que possível utilize injeção de dependência, ele vai tornar seu código mais limpo e desacoplado.

### Lei de Demeter
> A Lei de Demeter (LoD) ou princípio do menor conhecimento é um princípio que prega os seguintes pontos.

- Cada unidade deve ter conhecimento limitado sobre outras unidades: apenas unidades próximas se relacionam.
- Cada unidade deve apenas conversar com seus amigos.
- Não fale com estranhos, apenas fale com seus amigos imediatos.

## Regras sobre entendimento do código

- Seja consistente:
    - Se você executa algo de uma forma, execute todo o resto desta mesma forma. Seja consistente na forma com que aplica o código. Siga sempre o padrão definido.

- Utilize variáveis concisas: 
    - Opte por variáveis concisas, mesmo que resultem em um nome maior. Elas devem ser auto-explicativas.

- Obsessão primitiva:
    - No dia-a-dia tendemos a nos focar apenas em tipos primitivos (Built-in), causando uma obsessão pelos mesmos. Podemos criar e usar objetos de valor (Value Objects) para suprir melhor esta necessidade.

- Evite dependências lógicas: 
    - Não escreva métodos cujo funcionamento correto dependa de algo contido em sua classe.

- Evite condicionais negativas: 
    - A negação é dada por um sinal de exclamação (!) que muitas vezes pode ser imperceptível, ocasionando na má leitura do código.

## Regras de nomes

- Escolha nomes descritivos: 
    - Esolher bons nomes para classes, variáveis e métodos é essencial para um código limpo. Lembre-se que se você precisa explicar seu código, então algo pode ser melhorado nele.

- Faça distinções significantes: 
    - Utilize sempre nomes nos quais quem estiver lendo seu código possa diferenciar seu significado de outros possíveis nomes.

- Utilize nomes pronunciáveis e buscáveis: 

    - Evite utilizar nomes difíceis de pronunciar ou inventar nomes e conveções para variáveis, classes e métodos. Lembre-se sempre da linguagem ubíquoa e da importância dela no código.

- Evite uso excessivo de strings: 
    - Quem nunca perdeu horas procurando um BUG que era apenas um problema de comparação de string? Evite digitar a mesma string várias vezes, utilize constantes para isto.

## Regras para funções ou métodos

- Pequenas e com apenas um objetivo:
    - Mantenha suas funções ou métodos o menor possível. É mais fácil ter métodos menores e reutilizáveis do que tudo dentro de um método só.

- Utilize nomes descritivos:
    - A mesma regra dos nomes:  anteriormente vista aqui se aplica para este cenário. Mantenha nomes concisos, sem caracteres especiais.

- Opte por poucos parâmetros
    - Evite exigir muitos parâmetros para construção do objeto.

- Cuidado com efeitos colaterais: 
    - Evite que uma função altere valores de outra classe sem ser a dela. Isto é chamado de efeito colateral.

- Não tome decisões desnecessárias:
    - Não utilize os famosos "flags" para tomar decisões dentro dos métodos, divida-os em vários métodos ou até mesmo outras classes.

## Regras de comentários
- Um código bom é expressivo:
    - Teoricamente, se você precisa comentar uma parte do seu código, é por que algo está errado com ele, ele não está expressivo o suficiente.

- Não seja redundante:
    - Evite comentários que não fazem sentido algum ao contexto ou cenário.

- Não feche os comentários:
    - Não há necessidade de fechar os comentários.

- Evite códigos comentados:
    - Não deixe sujeira em seu código, ao invés de deixar algo comentado, remova ele.

- Inteção:
    - Um bom uso de comentários é sobre a intenção de um método, classe ou variável (Variável nem tanto).

- Esclarecimento:
    - Outro uso interessante para os comentários são esclarecimentos sobre o código.

## Estrutura do código

### Separe conceitos verticalmente
> Mantenha uma estrutura de pastas saudável e organizada. Não precisa criar uma pasta para cada arquivo, mas pode haver uma separação por contexto ou feature.

### Agrupe funcionalidades similares
> Se uma função pertence a um grupo dentro de um objeto, mantenha-as sempre por perto.

### Declare funções de cima para baixo
> Ordenar as funções também é importante. Além da sua ordem de grandeza, suas assinaturas também devem ter uma boa oganização.

### Mantenha poucas e curtas linhas
> Evite funções com linhas longas ou muitas linhas.

### Não quebre a identação
> Este item dispensa comentários. Um código não identado não pode ser enviado para o projeto.

### Objetos e estruturas
> Esconda estruturas internas
>>Este tópico abrange uma discussão extensa. Esconder a estrutura de um objeto, ou seja, privar as propridades relacioadas a dados dele, vai sempre trazer resultados positivos e negativos.

### Classe base não deve saber sobre suas derivadas

> Uma classe não deve saber sobre detalhes dos seus filhos. Nas verdade isto me soa tão estranho que não vejo um cenário onde uma classe pai consiga saber detalhes de seus filhos.

### Mais métodos, menos tomadas de decisão
> Já comentamos bastante isto na parte de OOP dos cursos, mas fica aqui o reforço, sempre opte por ter mais métodos, mais sobrecargas do que tomadas de decisão.

### Evite métodos estáticos
> Classes e métodos estáticos são difíceis de gerenciar, além de serem compartilhados entre a aplicação como um todo.

## Code smells

> Code Smells são alguns sintomas que podemos identificar e que nos remetem a uma má aplicação do Clean Code de uma forma geral.

### Rigidez
> Seu software é difícil de mudar. Qualquer mudança, por mínima que seja, causa uma cascata de outras mudanças.

### Fragilidade
> Uma simples mudança quebra seu software em diversos locais. É o famosos "cobre o pé, descobre a cabeça".

### Imobilidade
> Você não consegue reutilizar partes do seu código em outros projetos por que isto requer um esforço gigantes. Em resumo, tudo está muito acoplado.

### Complexidade desnecessária
> Você usa padrões e arquiteturas que tornam seu código mais burocrático do que efetivo. É o famoso "e se", onde pensamos em tudo que o software pode ter um dia e já "deixamos tudo pronto".

> "E se eu quiser voar com meu carro um dia?", bem, se um dia você quiser voar, aí você constrói as asas, mas se não vai precisar voar agora, foca em construir apenas o carro.

### Repetição desnecessária
> Você precisa repetir o mesmo código em diversos lugares.

### Opacidade
> Seu código é difícil de entender.
