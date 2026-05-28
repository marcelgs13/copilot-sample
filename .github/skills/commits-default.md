# Skill de Padronização de Commits

## Objetivo

Esta skill define um padrão para escrever mensagens de commit claras, organizadas e fáceis de entender, seguindo uma estrutura baseada em Conventional Commits.

## Escopo

Aplicar esta skill sempre que for criar, revisar ou sugerir mensagens de commit em projetos de software.

## Processo

1. Identificar o tipo da alteração feita no código.
2. Escolher o prefixo adequado para o commit.
3. Escrever uma mensagem curta, objetiva.
4. Quando necessário, adicionar uma descrição mais detalhada no corpo do commit.
5. Manter o padrão em todos os commits do projeto.

## Tipos de Commit

Use os seguintes prefixos:

* `feat`: nova funcionalidade
* `fix`: correção de bug
* `docs`: alteração em documentação
* `style`: mudanças de formatação, espaços, identação ou ponto e vírgula
* `refactor`: refatoração sem alterar comportamento
* `test`: criação ou alteração de testes
* `chore`: tarefas de manutenção ou configuração
* `perf`: melhoria de desempenho
* `build`: alterações em dependências ou processo de build
* `ci`: alterações em integração contínua

## Regras

* A mensagem deve ser curta e clara.
* Use letras minúsculas no tipo do commit.
* Use o formato:

```bash
tipo: descrição curta da alteração
```

* Não use ponto final no fim da mensagem curta.
* A descrição deve explicar o que foi alterado, não como foi alterado.
* Prefira mensagens como “adiciona”, “corrige”, “remove”, “atualiza”.
* Evite mensagens genéricas como `ajustes`, `alterações` ou `commit final`.

## Exemplos

```bash
feat: adiciona cadastro de usuários
```

```bash
fix: corrige erro ao validar login
```

```bash
docs: atualiza instruções de instalação
```

```bash
style: ajusta identação do arquivo de rotas
```

```bash
refactor: reorganiza lógica de autenticação
```

```bash
test: adiciona testes para criação de usuários
```

```bash
chore: atualiza dependências do projeto
```

## Exemplo com Escopo

Quando quiser indicar a parte do sistema afetada, use:

```bash
tipo(escopo): descrição curta
```

Exemplos:

```bash
feat(auth): adiciona login com token JWT
```

```bash
fix(api): corrige retorno da rota de usuários
```

```bash
docs(readme): atualiza comandos de execução
```

## Commits com Corpo

Use corpo quando a alteração precisar de mais explicação.

```bash
feat(users): adiciona listagem de usuários

Cria uma nova rota para retornar todos os usuários cadastrados no sistema.
A funcionalidade será utilizada na tela administrativa.
```

## Casos Especiais

### Correção simples

```bash
fix: corrige nome da variável de conexão
```

### Refatoração

```bash
refactor: separa regras de negócio em services
```

## Formato Final Recomendado

```bash
tipo(escopo opcional): descrição curta
```

Exemplo:

```bash
feat(frontend): adiciona tela de cadastro
```
