

> **Do iniciante ao avançado: tudo que você precisa saber para dominar a linguagem Go**

---

## Sumário

1. [Introdução ao Go](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#1-introdu%C3%A7%C3%A3o-ao-go)
2. [Instalação do Go](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#2-instala%C3%A7%C3%A3o-do-go)
3. [Estrutura de um Programa Go](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#3-estrutura-de-um-programa-go)
4. [Sintaxe Básica da Linguagem](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#4-sintaxe-b%C3%A1sica-da-linguagem)
5. [Tipos Primitivos](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#5-tipos-primitivos)
6. [Operadores](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#6-operadores)
7. [Controle de Fluxo](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#7-controle-de-fluxo)
8. [Loops](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#8-loops)
9. [Arrays](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#9-arrays)
10. [Slices](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#10-slices)
11. [Maps](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#11-maps)
12. [Funções](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#12-fun%C3%A7%C3%B5es)
13. [Estruturas (Structs)](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#13-estruturas-structs)
14. [Interfaces](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#14-interfaces)
15. [Ponteiros](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#15-ponteiros)
16. [Pacotes](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#16-pacotes)
17. [Módulos Go](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#17-m%C3%B3dulos-go)
18. [Manipulação de Arquivos](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#18-manipula%C3%A7%C3%A3o-de-arquivos)
19. [Tratamento de Erros](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#19-tratamento-de-erros)
20. [Concorrência — Goroutines e Channels](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#20-concorr%C3%AAncia--goroutines-e-channels)
21. [Goroutines Avançadas](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#21-goroutines-avan%C3%A7adas)
22. [Mutex e Sincronização](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#22-mutex-e-sincroniza%C3%A7%C3%A3o)
23. [JSON em Go](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#23-json-em-go)
24. [HTTP em Go](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#24-http-em-go)
25. [CLI em Go](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#25-cli-em-go)
26. [Boas Práticas](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#26-boas-pr%C3%A1ticas)
27. [Performance em Go](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#27-performance-em-go)
28. [Estrutura de Projetos Profissionais](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#28-estrutura-de-projetos-profissionais)
29. [Projeto Final — API REST Completa](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#29-projeto-final--api-rest-completa)
30. [Conclusão](https://claude.ai/chat/bcba9afe-9615-4ff0-8821-32762b9184a9#30-conclus%C3%A3o)

---

# 1. Introdução ao Go

## 1.1 História da Linguagem

Go (também chamado de Golang) é uma linguagem de programação compilada, estaticamente tipada e com foco em simplicidade, eficiência e concorrência. Ela foi criada dentro do Google e anunciada publicamente em novembro de **2009**.

A linguagem surgiu a partir de uma frustração dos seus criadores com o estado das linguagens existentes na época. Dentro do Google, grandes sistemas eram escritos em C++, Java e Python. C++ oferecia performance, mas tinha compilação lenta e complexidade excessiva. Java era mais produtivo, mas pesado. Python era produtivo, mas lento em produção.

A ideia era: criar uma linguagem com a performance de C/C++, a produtividade de Python, e suporte nativo a concorrência desde o primeiro dia.

A versão **1.0** foi lançada em março de **2012**, e desde então a linguagem manteve compatibilidade retroativa — código Go escrito em 2012 ainda compila e executa corretamente nas versões mais recentes.

## 1.2 Criadores da Linguagem

Go foi criado por três engenheiros do Google:

- **Robert Griesemer** — trabalhou no compilador V8 do JavaScript e em Java HotSpot
- **Rob Pike** — co-criador do sistema operacional Plan 9 e da codificação UTF-8
- **Ken Thompson** — co-criador do Unix e da linguagem B (precursora do C)

O trio tinha décadas de experiência em sistemas de grande escala. Isso explica muito das decisões de design da linguagem: pragmatismo acima de purismo.

## 1.3 Filosofia do Go

A filosofia central do Go pode ser resumida em algumas palavras: **simplicidade, legibilidade e composição**.

Os criadores do Go acreditam que:

- O código é lido muito mais vezes do que escrito
- Complexidade desnecessária é um inimigo
- A linguagem deve ser fácil de aprender e difícil de usar de forma errada
- Concorrência deve ser um cidadão de primeira classe

Por isso, Go deliberadamente **não possui** alguns recursos que outras linguagens têm:

- Sem herança de classe (apenas composição via embedding)
- Sem generics na versão original (adicionados apenas no Go 1.18)
- Sem sobrecarga de operadores
- Sem tratamento de exceções com try/catch
- Sem construtores implícitos

Cada uma dessas ausências foi uma escolha consciente, visando reduzir a complexidade e manter o código previsível e uniforme entre diferentes times.

## 1.4 Onde Go é Usado

Go é amplamente adotado em:

- **Infraestrutura de nuvem**: Docker, Kubernetes, Terraform, etcd são escritos em Go
- **Microsserviços e APIs**: muitas empresas migram serviços críticos para Go por causa da performance e facilidade de deployment
- **Ferramentas de linha de comando**: a CLI do GitHub, o Hugo (gerador de sites estáticos), e dezenas de outras ferramentas populares
- **Sistemas distribuídos**: CockroachDB, InfluxDB, e outros bancos de dados modernos
- **Segurança e redes**: muitas ferramentas de pentest e análise de rede são escritas em Go

Empresas que usam Go em produção: Google, Uber, Dropbox, Docker, Cloudflare, Twitch, SoundCloud, Mercado Livre, e muitas outras.

## 1.5 Vantagens e Desvantagens

### Vantagens

- **Compilação rápida**: projetos grandes compilam em segundos
- **Binário único**: o programa compilado é um único executável sem dependências externas
- **Concorrência nativa**: goroutines e channels tornam programas concorrentes muito mais simples
- **Garbage collector**: gerenciamento automático de memória sem a complexidade do C/C++
- **Tipagem estática**: erros de tipo são detectados em tempo de compilação
- **Padrão de formatação**: `gofmt` formata o código automaticamente, eliminando discussões de estilo
- **Biblioteca padrão rica**: HTTP, JSON, criptografia, e muito mais, tudo incluso

### Desvantagens

- **Generics tardios**: só foram adicionados no Go 1.18 (2022), o que ainda afeta o ecossistema
- **Sem exceções**: o tratamento explícito de erros pode ser verboso
- **Sem programação funcional avançada**: sem currying, pattern matching nativo, etc.
- **Runtime overhead**: o garbage collector e o runtime do Go têm um custo, não sendo ideal para sistemas de tempo real crítico
- **Ecossistema menor**: comparado a Java ou Python, embora esteja crescendo rapidamente

---

# 2. Instalação do Go

## 2.1 Instalando no Windows

1. Acesse o site oficial: https://go.dev/dl/
2. Baixe o instalador `.msi` para Windows (ex: `go1.22.0.windows-amd64.msi`)
3. Execute o instalador e siga as instruções
4. O instalador configura automaticamente as variáveis de ambiente `GOROOT` e atualiza o `PATH`

Verifique a instalação abrindo o Prompt de Comando ou PowerShell:

```bash
go version
# Saída esperada: go version go1.22.0 windows/amd64
```

## 2.2 Instalando no Linux

### Via gerenciador de pacotes (Ubuntu/Debian)

```bash
# Este método pode instalar uma versão desatualizada
sudo apt update
sudo apt install golang-go
```

### Via tarball (recomendado para versão mais recente)

```bash
# Baixe o arquivo tar.gz
wget https://go.dev/dl/go1.22.0.linux-amd64.tar.gz

# Remova instalação anterior (se houver)
sudo rm -rf /usr/local/go

# Extraia para /usr/local
sudo tar -C /usr/local -xzf go1.22.0.linux-amd64.tar.gz

# Adicione ao PATH (no ~/.bashrc ou ~/.zshrc)
echo 'export PATH=$PATH:/usr/local/go/bin' >> ~/.bashrc
source ~/.bashrc
```

## 2.3 Instalando no macOS

### Via Homebrew (mais simples)

```bash
brew install go
```

### Via instalador oficial

1. Acesse https://go.dev/dl/
2. Baixe o arquivo `.pkg` para macOS
3. Execute o instalador

## 2.4 Configuração do PATH e Variáveis de Ambiente

Go usa algumas variáveis de ambiente importantes:

| Variável | Descrição                      | Valor padrão típico |
| -------- | ------------------------------ | ------------------- |
| `GOROOT` | Onde o Go está instalado       | `/usr/local/go`     |
| `GOPATH` | Diretório de trabalho do Go    | `~/go`              |
| `GOBIN`  | Onde binários instalados ficam | `$GOPATH/bin`       |

Para configurar no Linux/macOS, adicione ao seu arquivo de configuração de shell (`~/.bashrc`, `~/.zshrc`, etc.):

```bash
export GOROOT=/usr/local/go
export GOPATH=$HOME/go
export GOBIN=$GOPATH/bin
export PATH=$PATH:$GOROOT/bin:$GOBIN
```

## 2.5 Testando a Instalação

```bash
# Verifica a versão instalada
go version

# Exibe todas as variáveis de ambiente do Go
go env

# Verifica variáveis específicas
go env GOROOT
go env GOPATH
```

### Seu primeiro programa

Crie um arquivo chamado `hello.go`:

```go
package main

import "fmt"

func main() {
    fmt.Println("Olá, Go!")
}
```

Execute-o:

```bash
# Executa diretamente (sem gerar binário)
go run hello.go

# Compila e gera um binário
go build hello.go
./hello  # No Windows: hello.exe
```

---

# 3. Estrutura de um Programa Go

## 3.1 Anatomia Completa

Vamos analisar o programa mais simples possível em Go, linha por linha:

```go
// hello.go

// Todo arquivo Go pertence a um pacote.
// O pacote "main" é especial: indica que este arquivo é um executável.
// Se o pacote fosse qualquer outro nome, seria uma biblioteca.
package main

// import declara os pacotes que este arquivo usa.
// "fmt" é o pacote de formatação de entrada e saída da biblioteca padrão.
import "fmt"

// func main() é o ponto de entrada do programa.
// Quando você executa o binário, o runtime do Go chama esta função primeiro.
// Ela não recebe argumentos e não retorna valores.
func main() {
    // fmt.Println imprime uma linha no terminal com quebra de linha no final.
    // O "." separa o pacote (fmt) da função (Println).
    fmt.Println("Olá, mundo!")
}
```

## 3.2 O Papel do `package main`

Em Go, todo arquivo de código-fonte começa com uma declaração de pacote. Os pacotes são a unidade fundamental de organização de código.

Existem dois tipos especiais de pacote:

**Pacote `main`**: Declara um executável. Deve conter uma função `main()`. Quando você compila, gera um binário executável.

**Qualquer outro pacote**: Declara uma biblioteca reutilizável. Não precisa de função `main()`. É importado por outros pacotes.

```go
// Este é um executável
package main

func main() {
    // código aqui
}
```

```go
// Este é uma biblioteca (pacote chamado "mathutils")
package mathutils

// Funções exportadas (com letra maiúscula) podem ser usadas por outros pacotes
func Soma(a, b int) int {
    return a + b
}

// Funções não exportadas (com letra minúscula) são privadas ao pacote
func subtracao(a, b int) int {
    return a - b
}
```

## 3.3 Como o Programa Inicia — O Runtime do Go

Quando você executa um programa Go, acontece o seguinte:

```
+------------------+
|   Seu binário    |
|                  |
|  1. Runtime Go   |  ← Inicializa o garbage collector, scheduler de goroutines
|  2. init()       |  ← Funções init() de todos os pacotes importados
|  3. main()       |  ← Sua função main
+------------------+
```

Funções `init()` são executadas automaticamente antes de `main()` e podem existir em qualquer pacote:

```go
package main

import "fmt"

// init() é chamada automaticamente antes de main()
// Você pode ter múltiplas funções init() no mesmo arquivo
func init() {
    fmt.Println("Executando init()...")
}

func main() {
    fmt.Println("Executando main()...")
}

// Saída:
// Executando init()...
// Executando main()...
```

## 3.4 Compilação em Go

Go é uma linguagem compilada. Isso significa que seu código-fonte é transformado em código de máquina antes de ser executado.

```bash
# Compila para o sistema operacional e arquitetura atual
go build main.go

# Compila para Linux 64-bit (cross-compilation!)
GOOS=linux GOARCH=amd64 go build -o meu_programa main.go

# Compila para Windows 64-bit
GOOS=windows GOARCH=amd64 go build -o meu_programa.exe main.go

# Compila para macOS ARM (Apple Silicon)
GOOS=darwin GOARCH=arm64 go build -o meu_programa main.go
```

A compilação cruzada (`cross-compilation`) é um dos pontos fortes do Go. Você pode compilar para qualquer plataforma suportada diretamente do seu computador, sem precisar de uma máquina separada.

### Como a compilação funciona internamente

```
Código-fonte (.go)
        ↓
    Análise Léxica (tokenização)
        ↓
    Análise Sintática (AST - Abstract Syntax Tree)
        ↓
    Análise Semântica (verificação de tipos)
        ↓
    Geração de SSA (Static Single Assignment)
        ↓
    Otimizações
        ↓
    Geração de código de máquina
        ↓
    Linkagem (linking)
        ↓
    Binário executável
```

Uma das razões pelas quais o Go compila tão rápido é que ele evita inclusões de cabeçalho circulares (diferente do C/C++) e possui um sistema de importação eficiente.

## 3.5 `go run` vs `go build`

```bash
# go run: compila e executa em memória (não gera arquivo)
# Bom para desenvolvimento e scripts
go run main.go

# go build: compila e gera um binário
# Bom para produção e distribuição
go build -o meuapp main.go
./meuapp

# go install: compila e instala o binário em $GOBIN
go install .
```

---

# 4. Sintaxe Básica da Linguagem

## 4.1 Declaração de Variáveis

Go é estaticamente tipado, mas oferece inferência de tipo. Você tem várias formas de declarar variáveis:

### Forma completa com `var`

```go
package main

import "fmt"

func main() {
    // Forma completa: var nome tipo = valor
    var nome string = "João"
    var idade int = 30
    var altura float64 = 1.75
    var ativo bool = true

    fmt.Println(nome, idade, altura, ativo)
    // Saída: João 30 1.75 true
}
```

### Declaração sem valor inicial (zero value)

Em Go, toda variável tem um valor zero quando declarada sem inicialização:

```go
package main

import "fmt"

func main() {
    var nome string   // zero value de string é ""
    var idade int     // zero value de int é 0
    var preco float64 // zero value de float64 é 0.0
    var ativo bool    // zero value de bool é false

    // Ponteiros, slices, maps, channels e funções têm zero value nil
    var ponteiro *int  // zero value é nil

    fmt.Printf("nome: %q\n", nome)       // nome: ""
    fmt.Printf("idade: %d\n", idade)     // idade: 0
    fmt.Printf("preco: %.1f\n", preco)   // preco: 0.0
    fmt.Printf("ativo: %t\n", ativo)     // ativo: false
    fmt.Printf("ponteiro: %v\n", ponteiro) // ponteiro: <nil>
}
```

Essa característica é muito importante: **não existem variáveis não inicializadas em Go**. Isso elimina toda uma classe de bugs comuns em C/C++.

### Inferência de tipo com `var`

```go
package main

import "fmt"

func main() {
    // O tipo é inferido do valor atribuído
    var nome = "Maria"     // Go infere: string
    var idade = 25         // Go infere: int
    var preco = 99.90      // Go infere: float64
    var ativo = true       // Go infere: bool

    fmt.Printf("tipo de nome: %T\n", nome)   // tipo de nome: string
    fmt.Printf("tipo de idade: %T\n", idade) // tipo de idade: int
    fmt.Printf("tipo de preco: %T\n", preco) // tipo de preco: float64
}
```

### Operador `:=` (short variable declaration)

Esta é a forma mais comum de declarar variáveis dentro de funções:

```go
package main

import "fmt"

func main() {
    // := declara E inicializa a variável
    // Só funciona dentro de funções
    nome := "Carlos"
    idade := 28
    preco := 150.50
    ativo := false

    fmt.Println(nome, idade, preco, ativo)

    // Declaração múltipla com :=
    x, y, z := 10, 20, 30
    fmt.Println(x, y, z)

    // Útil para capturar múltiplos retornos de funções
    // (veremos mais sobre isso em funções)
    resultado, err := dividir(10, 2)
    if err != nil {
        fmt.Println("Erro:", err)
        return
    }
    fmt.Println("Resultado:", resultado)
}

func dividir(a, b float64) (float64, error) {
    if b == 0 {
        return 0, fmt.Errorf("divisão por zero")
    }
    return a / b, nil
}
```

### Declaração de bloco com `var`

```go
package main

import "fmt"

// Variáveis de pacote (globais) devem usar var
var (
    AppNome    = "MeuApp"
    AppVersao  = "1.0.0"
    AppDebug   = false
)

func main() {
    // Bloco var dentro de função
    var (
        nome  = "Ana"
        idade = 32
        email = "ana@email.com"
    )

    fmt.Println(AppNome, AppVersao)
    fmt.Println(nome, idade, email)
}
```

## 4.2 Tipos — Uma Visão Geral

Go tem um sistema de tipos rico. Os principais tipos são:

```
Tipos Básicos:
├── Numéricos inteiros: int, int8, int16, int32, int64
│                       uint, uint8, uint16, uint32, uint64, uintptr
├── Numéricos flutuantes: float32, float64
├── Complexos: complex64, complex128
├── Booleano: bool
└── String: string

Tipos Compostos:
├── Array: [N]T
├── Slice: []T
├── Map: map[K]V
├── Struct: struct{...}
├── Ponteiro: *T
├── Função: func(...)
├── Interface: interface{...}
└── Channel: chan T
```

## 4.3 Constantes

Constantes são valores imutáveis definidos em tempo de compilação:

```go
package main

import "fmt"

// Constantes de pacote
const PI = 3.14159265358979
const NomeApp = "MeuSistema"
const VersaoMajor = 1

// Bloco de constantes
const (
    StatusAtivo   = "ativo"
    StatusInativo = "inativo"
    StatusPendente = "pendente"

    // iota é um enumerador especial do Go
    // começa em 0 e incrementa a cada linha dentro de const()
    Segunda = iota // 0
    Terca          // 1
    Quarta         // 2
    Quinta         // 3
    Sexta          // 4
    Sabado         // 5
    Domingo        // 6
)

// Usando iota com expressões
const (
    _           = iota             // ignorar o primeiro valor (0)
    KB = 1 << (10 * iota)          // 1 << 10 = 1024
    MB                             // 1 << 20 = 1048576
    GB                             // 1 << 30 = 1073741824
    TB                             // 1 << 40
)

func main() {
    fmt.Println("PI:", PI)
    fmt.Println("App:", NomeApp)
    fmt.Println("Dias:", Segunda, Terca, Quarta)

    fmt.Printf("KB = %d\n", KB) // 1024
    fmt.Printf("MB = %d\n", MB) // 1048576
    fmt.Printf("GB = %d\n", GB) // 1073741824

    // Constantes tipadas
    const MaxConexoes int = 100
    const TaxaJuros float64 = 0.05

    fmt.Println(MaxConexoes, TaxaJuros)
}
```

### Diferença entre constante e variável

```go
package main

func main() {
    // Variável: pode ser alterada
    var contador int = 0
    contador = 10
    contador++

    // Constante: não pode ser alterada
    const MaxTentativas = 3

    // Isso causaria erro de compilação:
    // MaxTentativas = 5  // ERRO: cannot assign to MaxTentativas

    // Constantes podem ser usadas em expressões de tipos
    var tentativas [MaxTentativas]int // array de tamanho 3
    _ = tentativas
    _ = contador
}
```

---

# 5. Tipos Primitivos

## 5.1 Tipos Inteiros

Go possui vários tipos inteiros. Entender cada um é importante para escrever código eficiente:

### Inteiros com sinal

```go
package main

import (
    "fmt"
    "math"
)

func main() {
    // int: tamanho depende da plataforma (32 ou 64 bits)
    // Na maioria dos sistemas modernos: 64 bits
    var i int = 42

    // int8: 8 bits, range de -128 a 127
    var i8 int8 = 127
    // var i8Overflow int8 = 128  // ERRO: valor muito grande

    // int16: 16 bits, range de -32768 a 32767
    var i16 int16 = 32767

    // int32: 32 bits, range de -2147483648 a 2147483647
    // int32 é um alias para 'rune' (caractere Unicode)
    var i32 int32 = 2147483647

    // int64: 64 bits, range enorme
    var i64 int64 = 9223372036854775807

    fmt.Println(i, i8, i16, i32, i64)

    // Valores máximos usando o pacote math
    fmt.Printf("int8  max: %d\n", math.MaxInt8)   // 127
    fmt.Printf("int16 max: %d\n", math.MaxInt16)  // 32767
    fmt.Printf("int32 max: %d\n", math.MaxInt32)  // 2147483647
    fmt.Printf("int64 max: %d\n", math.MaxInt64)  // 9223372036854775807
}
```

### Inteiros sem sinal

```go
package main

import (
    "fmt"
    "math"
)

func main() {
    // uint: unsigned int (sem sinal), 0 a 2^32-1 ou 2^64-1
    var u uint = 42

    // uint8: 0 a 255 — também chamado de 'byte'
    var u8 uint8 = 255
    var b byte = 255 // byte é um alias para uint8

    // uint16: 0 a 65535
    var u16 uint16 = 65535

    // uint32: 0 a 4294967295
    var u32 uint32 = 4294967295

    // uint64: 0 a 18446744073709551615
    var u64 uint64 = math.MaxUint64

    fmt.Println(u, u8, b, u16, u32, u64)

    // uintptr: tamanho suficiente para armazenar um ponteiro
    // Usado em código de baixo nível
    var ptr uintptr = 0xDEADBEEF
    fmt.Printf("ptr: 0x%X\n", ptr)
}
```

### Operações com inteiros

```go
package main

import "fmt"

func main() {
    a := 17
    b := 5

    fmt.Println("a + b =", a+b) // 22
    fmt.Println("a - b =", a-b) // 12
    fmt.Println("a * b =", a*b) // 85
    fmt.Println("a / b =", a/b) // 3 (divisão inteira!)
    fmt.Println("a % b =", a%b) // 2 (resto da divisão)

    // Atenção: divisão inteira descarta a parte decimal
    fmt.Println(7 / 2)   // 3, NÃO 3.5
    fmt.Println(7.0 / 2) // 3.5 (pelo menos um float)

    // Overflow — cuidado!
    var x int8 = 127
    x++
    fmt.Println(x) // -128 (overflow! wraps around)
}
```

## 5.2 Tipos de Ponto Flutuante

```go
package main

import (
    "fmt"
    "math"
)

func main() {
    // float32: precisão de ~7 dígitos decimais
    var f32 float32 = 3.14159265358979323846
    fmt.Printf("float32: %.20f\n", f32)
    // Saída: float32: 3.14159274101257324219 (perda de precisão!)

    // float64: precisão de ~15-17 dígitos decimais
    // Este é o tipo padrão para literais de ponto flutuante
    var f64 float64 = 3.14159265358979323846
    fmt.Printf("float64: %.20f\n", f64)
    // Saída: float64: 3.14159265358979323846

    // Literais de ponto flutuante
    a := 1.5        // float64
    b := 1.5e3      // 1500.0 (notação científica)
    c := 2.5e-2     // 0.025
    d := 0.5        // float64
    e := .5         // também válido: float64

    fmt.Println(a, b, c, d, e)

    // Constantes matemáticas
    fmt.Println("π:", math.Pi)          // 3.141592653589793
    fmt.Println("e:", math.E)           // 2.718281828459045
    fmt.Println("√2:", math.Sqrt2)      // 1.4142135623730951

    // Funções matemáticas
    fmt.Println(math.Sqrt(16.0))        // 4
    fmt.Println(math.Pow(2, 10))        // 1024
    fmt.Println(math.Abs(-42.5))        // 42.5
    fmt.Println(math.Floor(3.7))        // 3
    fmt.Println(math.Ceil(3.2))         // 4
    fmt.Println(math.Round(3.5))        // 4

    // Verificações especiais
    fmt.Println(math.IsNaN(math.NaN()))   // true
    fmt.Println(math.IsInf(math.Inf(1), 1)) // true

    // Cuidado com comparações de floats!
    x := 0.1 + 0.2
    fmt.Println(x == 0.3)              // false! (problema de representação binária)
    fmt.Printf("%.20f\n", x)           // 0.30000000000000004440...

    // Forma correta de comparar floats
    const epsilon = 1e-10
    fmt.Println(math.Abs(x-0.3) < epsilon) // true
}
```

## 5.3 O Tipo String

Strings em Go são sequências imutáveis de bytes. Elas são codificadas em UTF-8 por padrão.

```go
package main

import (
    "fmt"
    "strings"
    "unicode/utf8"
)

func main() {
    // Declaração de strings
    s1 := "Olá, mundo!"
    s2 := `Esta é uma
string raw que pode ter
múltiplas linhas e "aspas"
sem precisar escapar`

    fmt.Println(s1)
    fmt.Println(s2)

    // Strings são imutáveis
    // s1[0] = 'o'  // ERRO: cannot assign to s1[0]

    // Concatenação com +
    nome := "João"
    sobrenome := "Silva"
    nomeCompleto := nome + " " + sobrenome
    fmt.Println(nomeCompleto) // João Silva

    // Comprimento em bytes (não em caracteres Unicode!)
    s := "Olá"
    fmt.Println("len bytes:", len(s))                   // 5 (ó ocupa 2 bytes em UTF-8)
    fmt.Println("len runes:", utf8.RuneCountInString(s)) // 3 (3 caracteres)

    // Iteração byte a byte
    fmt.Println("\nIteração por bytes:")
    for i := 0; i < len(s); i++ {
        fmt.Printf("  s[%d] = %d (%c)\n", i, s[i], s[i])
    }

    // Iteração por rune (caractere Unicode) — forma correta
    fmt.Println("\nIteração por runes:")
    for i, r := range s {
        fmt.Printf("  índice=%d, rune=%d (%c)\n", i, r, r)
    }

    // Funções do pacote strings
    texto := "  Hello, World!  "
    fmt.Println(strings.TrimSpace(texto))              // "Hello, World!"
    fmt.Println(strings.ToUpper("golang"))             // "GOLANG"
    fmt.Println(strings.ToLower("GOLANG"))             // "golang"
    fmt.Println(strings.Contains("golang", "lang"))   // true
    fmt.Println(strings.HasPrefix("golang", "go"))    // true
    fmt.Println(strings.HasSuffix("golang", "lang"))  // true
    fmt.Println(strings.Replace("aabaa", "a", "o", 2)) // "oobaa" (substituir 2 ocorrências)
    fmt.Println(strings.ReplaceAll("aabaa", "a", "o")) // "ooboo"
    fmt.Println(strings.Split("a,b,c", ","))           // ["a" "b" "c"]
    fmt.Println(strings.Join([]string{"a","b","c"}, "-")) // "a-b-c"
    fmt.Println(strings.Count("golang", "g"))           // 2
    fmt.Println(strings.Index("golang", "lang"))        // 2
    fmt.Println(strings.TrimPrefix("golang", "go"))     // "lang"
}
```

### Conversão entre string e bytes/runes

```go
package main

import "fmt"

func main() {
    s := "Olá, Go!"

    // String para []byte
    bytes := []byte(s)
    fmt.Println("bytes:", bytes)
    // [79 108 195 161 44 32 71 111 33]

    // []byte para string
    s2 := string(bytes)
    fmt.Println("string:", s2) // Olá, Go!

    // String para []rune (para trabalhar com caracteres Unicode)
    runes := []rune(s)
    fmt.Println("runes:", runes)
    // [79 108 225 44 32 71 111 33]

    // []rune para string
    s3 := string(runes)
    fmt.Println("string:", s3) // Olá, Go!

    // int para string (converte o código Unicode para caractere)
    r := rune(65)
    fmt.Println(string(r)) // A

    // Para converter número para string, use fmt.Sprintf ou strconv
    n := 42
    // ERRADO: string(n) não faz o que você espera
    // CORRETO:
    numStr := fmt.Sprintf("%d", n) // "42"
    fmt.Println(numStr)
}
```

### Construção eficiente de strings com strings.Builder

```go
package main

import (
    "fmt"
    "strings"
)

func main() {
    // Forma ineficiente (cria muitas strings intermediárias)
    resultado := ""
    for i := 0; i < 5; i++ {
        resultado += fmt.Sprintf("item%d ", i)
    }
    fmt.Println(resultado)

    // Forma eficiente com strings.Builder
    var sb strings.Builder
    for i := 0; i < 5; i++ {
        fmt.Fprintf(&sb, "item%d ", i)
    }
    fmt.Println(sb.String())
    // Ambas produzem: item0 item1 item2 item3 item4
}
```

## 5.4 O Tipo Boolean

```go
package main

import "fmt"

func main() {
    // Declaração
    var verdadeiro bool = true
    var falso bool = false
    inferido := true

    fmt.Println(verdadeiro, falso, inferido)

    // Operadores lógicos
    fmt.Println(true && true)   // true  (AND)
    fmt.Println(true && false)  // false (AND)
    fmt.Println(false || true)  // true  (OR)
    fmt.Println(false || false) // false (OR)
    fmt.Println(!true)          // false (NOT)
    fmt.Println(!false)         // true  (NOT)

    // Short-circuit evaluation
    // Em Go, assim como na maioria das linguagens:
    // false && qualquer_coisa = false (não avalia o segundo)
    // true  || qualquer_coisa = true  (não avalia o segundo)

    x := 0
    // A função "divide" não é chamada porque false && ... = false
    resultado := false && (x/0 == 1) // não panic!
    fmt.Println(resultado)

    // Zero value de bool é false
    var b bool
    fmt.Println(b) // false
}
```

## 5.5 byte e rune

```go
package main

import "fmt"

func main() {
    // byte é um alias para uint8
    // Representa um único byte (valor 0-255)
    var b byte = 65
    fmt.Println(b)        // 65
    fmt.Printf("%c\n", b) // A

    // rune é um alias para int32
    // Representa um único ponto de código Unicode
    var r rune = 'A'          // literais de caractere usam aspas simples
    var r2 rune = '🚀'        // emojis também são runes!
    var r3 rune = '中'         // caracteres chineses também

    fmt.Printf("rune: %d (%c)\n", r, r)   // rune: 65 (A)
    fmt.Printf("rune: %d (%c)\n", r2, r2) // rune: 128640 (🚀)
    fmt.Printf("rune: %d (%c)\n", r3, r3) // rune: 20013 (中)

    // Literais de caractere
    a := 'a'        // rune
    newline := '\n' // caractere de nova linha
    tab := '\t'     // caractere de tabulação
    _ = a
    _ = newline
    _ = tab

    // Por que isso importa?
    // Em Go, uma string é uma sequência de bytes, não de runes
    // Caracteres Unicode podem ocupar 1-4 bytes
    s := "Hello, 世界"
    fmt.Println("bytes:", len(s))         // 13 (! não 9)
    fmt.Println("caracteres:", len([]rune(s))) // 9
}
```

---

# 6. Operadores

## 6.1 Operadores Aritméticos

```go
package main

import "fmt"

func main() {
    a, b := 10, 3

    fmt.Println("Adição:      ", a+b)  // 13
    fmt.Println("Subtração:   ", a-b)  // 7
    fmt.Println("Multiplicação:", a*b) // 30
    fmt.Println("Divisão:     ", a/b)  // 3 (inteira!)
    fmt.Println("Módulo:      ", a%b)  // 1

    // Operadores de incremento e decremento
    // Em Go, ++ e -- são STATEMENTS, não expressões
    // Isso significa: x++ é válido, mas y = x++ NÃO é
    x := 5
    x++  // x = 6
    x--  // x = 5
    // y := x++  // ERRO em Go!

    fmt.Println(x)

    // Operadores de atribuição combinada
    n := 10
    n += 5  // n = n + 5 = 15
    n -= 3  // n = n - 3 = 12
    n *= 2  // n = n * 2 = 24
    n /= 4  // n = n / 4 = 6
    n %= 4  // n = n % 4 = 2
    fmt.Println(n)

    // Divisão de floats
    x1, x2 := 10.0, 3.0
    fmt.Printf("%.4f\n", x1/x2) // 3.3333
}
```

## 6.2 Operadores de Comparação

```go
package main

import "fmt"

func main() {
    a, b := 10, 20

    fmt.Println("a == b:", a == b) // false
    fmt.Println("a != b:", a != b) // true
    fmt.Println("a < b: ", a < b)  // true
    fmt.Println("a > b: ", a > b)  // false
    fmt.Println("a <= b:", a <= b) // true
    fmt.Println("a >= b:", a >= b) // false

    // Strings podem ser comparadas lexicograficamente
    s1, s2 := "apple", "banana"
    fmt.Println("s1 == s2:", s1 == s2) // false
    fmt.Println("s1 < s2: ", s1 < s2)  // true ("apple" vem antes de "banana")

    // Comparação de structs
    type Ponto struct {
        X, Y int
    }
    p1 := Ponto{1, 2}
    p2 := Ponto{1, 2}
    p3 := Ponto{3, 4}
    fmt.Println("p1 == p2:", p1 == p2) // true
    fmt.Println("p1 == p3:", p1 == p3) // false

    // Slices, maps e funções NÃO podem ser comparados com ==
    // (exceto com nil)
    s := []int{1, 2, 3}
    fmt.Println("s == nil:", s == nil) // false
}
```

## 6.3 Operadores Lógicos

```go
package main

import "fmt"

func main() {
    // AND lógico: && — ambos devem ser true
    fmt.Println(true && true)   // true
    fmt.Println(true && false)  // false
    fmt.Println(false && false) // false

    // OR lógico: || — pelo menos um deve ser true
    fmt.Println(true || false)  // true
    fmt.Println(false || false) // false
    fmt.Println(true || true)   // true

    // NOT lógico: !
    fmt.Println(!true)  // false
    fmt.Println(!false) // true

    // Exemplo prático
    idade := 20
    temCarteira := true

    podeDirigir := idade >= 18 && temCarteira
    fmt.Println("Pode dirigir:", podeDirigir) // true

    // Short-circuit: Go para de avaliar assim que o resultado é determinado
    contadorChamadas := 0

    avaliar := func() bool {
        contadorChamadas++
        return true
    }

    // false && ... nunca chama avaliar()
    resultado := false && avaliar()
    fmt.Println("contador:", contadorChamadas, "resultado:", resultado)
    // contador: 0 resultado: false

    // true || ... nunca chama avaliar()
    resultado = true || avaliar()
    fmt.Println("contador:", contadorChamadas, "resultado:", resultado)
    // contador: 0 resultado: true
}
```

## 6.4 Operadores Bitwise

```go
package main

import "fmt"

func main() {
    a := 0b1010 // 10 em binário
    b := 0b1100 // 12 em binário

    // AND bitwise: bits iguais a 1 em AMBOS
    fmt.Printf("a & b  = %04b = %d\n", a&b, a&b)   // 1000 = 8

    // OR bitwise: bits iguais a 1 em PELO MENOS UM
    fmt.Printf("a | b  = %04b = %d\n", a|b, a|b)   // 1110 = 14

    // XOR bitwise: bits iguais a 1 em EXATAMENTE UM
    fmt.Printf("a ^ b  = %04b = %d\n", a^b, a^b)   // 0110 = 6

    // AND NOT (bit clear): bits de a onde b tem 0
    fmt.Printf("a &^ b = %04b = %d\n", a&^b, a&^b) // 0010 = 2

    // Shift left: multiplica por 2^n
    fmt.Printf("a << 1 = %04b = %d\n", a<<1, a<<1) // 10100 = 20
    fmt.Printf("a << 2 = %04b = %d\n", a<<2, a<<2) // 101000 = 40

    // Shift right: divide por 2^n
    fmt.Printf("a >> 1 = %04b = %d\n", a>>1, a>>1) // 0101 = 5

    // Aplicação prática: flags de permissão
    const (
        Leitura  = 1 << iota // 1 (001)
        Escrita               // 2 (010)
        Execucao              // 4 (100)
    )

    permissao := Leitura | Escrita // 3 (011)
    fmt.Println("Tem leitura: ", permissao&Leitura != 0)  // true
    fmt.Println("Tem escrita: ", permissao&Escrita != 0)  // true
    fmt.Println("Tem execução:", permissao&Execucao != 0) // false

    // Adicionar permissão
    permissao |= Execucao
    fmt.Println("Após adicionar execução:", permissao&Execucao != 0) // true

    // Remover permissão
    permissao &^= Escrita
    fmt.Println("Após remover escrita:", permissao&Escrita != 0) // false
}
```

---

# 7. Controle de Fluxo

## 7.1 if / else if / else

```go
package main

import "fmt"

func main() {
    // if simples
    temperatura := 25
    if temperatura > 30 {
        fmt.Println("Está quente!")
    }

    // if / else
    nota := 75
    if nota >= 60 {
        fmt.Println("Aprovado")
    } else {
        fmt.Println("Reprovado")
    }

    // if / else if / else
    hora := 14

    if hora < 12 {
        fmt.Println("Bom dia!")
    } else if hora < 18 {
        fmt.Println("Boa tarde!")
    } else {
        fmt.Println("Boa noite!")
    }

    // Característica especial do Go: if com inicialização
    // A variável declarada na inicialização só existe dentro do if
    if resultado, err := calcular(10, 0); err != nil {
        fmt.Println("Erro:", err)
    } else {
        fmt.Println("Resultado:", resultado)
    }
    // resultado e err não existem aqui

    // Outro exemplo prático
    if valor, ok := map[string]int{"a": 1}["a"]; ok {
        fmt.Println("Valor encontrado:", valor)
    } else {
        fmt.Println("Chave não encontrada")
    }
}

func calcular(a, b float64) (float64, error) {
    if b == 0 {
        return 0, fmt.Errorf("divisão por zero")
    }
    return a / b, nil
}
```

## 7.2 switch

O `switch` em Go é muito mais poderoso e flexível do que em C/Java:

```go
package main

import (
    "fmt"
    "time"
)

func main() {
    // switch básico — sem break necessário! Não tem fall-through por padrão
    dia := 3
    switch dia {
    case 1:
        fmt.Println("Domingo")
    case 2:
        fmt.Println("Segunda")
    case 3:
        fmt.Println("Terça")
    case 4:
        fmt.Println("Quarta")
    case 5:
        fmt.Println("Quinta")
    case 6:
        fmt.Println("Sexta")
    case 7:
        fmt.Println("Sábado")
    default:
        fmt.Println("Dia inválido")
    }

    // Múltiplos valores no mesmo case
    diaSemana := time.Now().Weekday()
    switch diaSemana {
    case time.Saturday, time.Sunday:
        fmt.Println("Fim de semana!")
    default:
        fmt.Println("Dia de trabalho")
    }

    // switch sem expressão (como if-else)
    nota := 85
    switch {
    case nota >= 90:
        fmt.Println("A")
    case nota >= 80:
        fmt.Println("B")
    case nota >= 70:
        fmt.Println("C")
    case nota >= 60:
        fmt.Println("D")
    default:
        fmt.Println("F")
    }

    // switch com inicialização
    switch x := calcularValor(); {
    case x > 0:
        fmt.Println("Positivo:", x)
    case x < 0:
        fmt.Println("Negativo:", x)
    default:
        fmt.Println("Zero")
    }

    // fallthrough: força a execução do próximo case
    n := 2
    switch n {
    case 1:
        fmt.Println("um")
        fallthrough
    case 2:
        fmt.Println("dois") // executado
        fallthrough
    case 3:
        fmt.Println("três") // também executado por causa do fallthrough
    case 4:
        fmt.Println("quatro") // NÃO executado
    }
}

func calcularValor() int {
    return 42
}
```

### Type Switch

O type switch é único do Go e permite verificar o tipo de uma interface:

```go
package main

import "fmt"

func descreverTipo(i interface{}) {
    switch v := i.(type) {
    case int:
        fmt.Printf("int: %d (dobro = %d)\n", v, v*2)
    case string:
        fmt.Printf("string: %q (comprimento = %d)\n", v, len(v))
    case bool:
        fmt.Printf("bool: %t\n", v)
    case []int:
        fmt.Printf("[]int com %d elementos: %v\n", len(v), v)
    case nil:
        fmt.Println("nil")
    default:
        fmt.Printf("tipo desconhecido: %T\n", v)
    }
}

func main() {
    descreverTipo(42)
    descreverTipo("Olá, Go!")
    descreverTipo(true)
    descreverTipo([]int{1, 2, 3})
    descreverTipo(nil)
    descreverTipo(3.14)
}
```

---

# 8. Loops

## 8.1 O `for` — único loop em Go

Go tem apenas um tipo de loop: o `for`. Mas ele é tão flexível que substitui todos os outros.

### for tradicional (como C)

```go
package main

import "fmt"

func main() {
    // for com init; condição; post
    for i := 0; i < 5; i++ {
        fmt.Println(i)
    }
    // Saída: 0 1 2 3 4

    // Contagem regressiva
    for i := 5; i > 0; i-- {
        fmt.Print(i, " ")
    }
    fmt.Println()
    // Saída: 5 4 3 2 1

    // Step de 2
    for i := 0; i <= 10; i += 2 {
        fmt.Print(i, " ")
    }
    fmt.Println()
    // Saída: 0 2 4 6 8 10
}
```

### for como while

```go
package main

import "fmt"

func main() {
    // for com apenas condição (como while em outras linguagens)
    n := 1
    for n < 100 {
        n *= 2
    }
    fmt.Println(n) // 128

    // Lendo até encontrar uma condição
    soma := 0
    numeros := []int{3, 7, 2, 9, 4, 1, 8}
    i := 0
    for i < len(numeros) && soma < 15 {
        soma += numeros[i]
        i++
    }
    fmt.Println("Soma:", soma) // 21 (parou ao ultrapassar 15)
}
```

### for infinito

```go
package main

import (
    "fmt"
    "time"
)

func main() {
    // for sem condição = loop infinito
    // Sempre precisa de um break ou return para sair

    tentativas := 0
    for {
        tentativas++
        if tentativas >= 3 {
            fmt.Println("Máximo de tentativas atingido")
            break
        }
        fmt.Println("Tentativa", tentativas)
    }

    // Loop com continue (pula o resto da iteração atual)
    fmt.Println("\nNúmeros ímpares:")
    for i := 0; i < 10; i++ {
        if i%2 == 0 {
            continue // pula números pares
        }
        fmt.Print(i, " ")
    }
    fmt.Println()
    // Saída: 1 3 5 7 9

    // Simulação de ticker
    tick := 0
    for {
        tick++
        time.Sleep(10 * time.Millisecond)
        if tick >= 3 {
            fmt.Println("Parando após", tick, "ticks")
            break
        }
    }
}
```

### Labels para break e continue

```go
package main

import "fmt"

func main() {
    // Labels permitem sair de loops aninhados
outer:
    for i := 0; i < 3; i++ {
        for j := 0; j < 3; j++ {
            if i == 1 && j == 1 {
                fmt.Println("Saindo do loop externo em i=1, j=1")
                break outer // sai do loop marcado como "outer"
            }
            fmt.Printf("i=%d, j=%d\n", i, j)
        }
    }

    // continue com label
    fmt.Println("\nCom continue label:")
loop:
    for i := 0; i < 3; i++ {
        for j := 0; j < 3; j++ {
            if j == 1 {
                continue loop // vai para a próxima iteração do loop externo
            }
            fmt.Printf("i=%d, j=%d\n", i, j)
        }
    }
}
```

## 8.2 for range

O `for range` itera sobre arrays, slices, maps, strings e channels:

```go
package main

import "fmt"

func main() {
    // Range em slice
    frutas := []string{"maçã", "banana", "laranja"}

    // Com índice e valor
    for i, fruta := range frutas {
        fmt.Printf("[%d] %s\n", i, fruta)
    }

    // Só valor (ignorando índice com _)
    for _, fruta := range frutas {
        fmt.Println(fruta)
    }

    // Só índice
    for i := range frutas {
        fmt.Println(i)
    }

    // Range em array
    numeros := [5]int{10, 20, 30, 40, 50}
    for i, n := range numeros {
        fmt.Printf("numeros[%d] = %d\n", i, n)
    }

    // Range em map (ordem não garantida!)
    capitais := map[string]string{
        "Brasil":    "Brasília",
        "Argentina": "Buenos Aires",
        "Chile":     "Santiago",
    }
    for pais, capital := range capitais {
        fmt.Printf("%s → %s\n", pais, capital)
    }

    // Range em string (itera por rune, não por byte)
    for i, r := range "Olá" {
        fmt.Printf("índice=%d, rune=%d, char=%c\n", i, r, r)
    }
    // índice=0, rune=79,  char=O
    // índice=1, rune=108, char=l
    // índice=2, rune=225, char=á  (índice 2, mas 'á' ocupa bytes 2 e 3)

    // Range em channel (veremos mais adiante)
    ch := make(chan int, 3)
    ch <- 1
    ch <- 2
    ch <- 3
    close(ch)
    for v := range ch {
        fmt.Print(v, " ")
    }
    fmt.Println()
}
```

---

# 9. Arrays

## 9.1 O que são Arrays em Go

Arrays em Go são sequências de tamanho fixo de elementos do mesmo tipo. O tamanho faz parte do tipo: `[5]int` é um tipo diferente de `[10]int`.

```go
package main

import "fmt"

func main() {
    // Declaração com tamanho e tipo
    var arr [5]int
    fmt.Println(arr) // [0 0 0 0 0] (zero value para todos os elementos)

    // Declaração com inicialização
    primos := [5]int{2, 3, 5, 7, 11}
    fmt.Println(primos) // [2 3 5 7 11]

    // O compilador conta os elementos automaticamente com ...
    vogais := [...]string{"a", "e", "i", "o", "u"}
    fmt.Println(len(vogais)) // 5

    // Inicialização por índice
    especial := [5]int{1: 10, 3: 30}
    fmt.Println(especial) // [0 10 0 30 0]

    // Acesso por índice
    fmt.Println(primos[0]) // 2 (primeiro elemento)
    fmt.Println(primos[4]) // 11 (último elemento)

    // Modificação
    primos[0] = 1
    fmt.Println(primos) // [1 3 5 7 11]

    // Tamanho com len()
    fmt.Println(len(primos)) // 5
}
```

## 9.2 Arrays são Valores (não Referências)

Esta é uma distinção crucial: em Go, arrays são **copiados** quando atribuídos ou passados para funções.

```go
package main

import "fmt"

func main() {
    original := [3]int{1, 2, 3}

    // Cópia — modificar copia não afeta original
    copia := original
    copia[0] = 100

    fmt.Println("original:", original) // [1 2 3] (não mudou!)
    fmt.Println("copia:   ", copia)    // [100 2 3]

    // Isso tem implicações em funções:
    modificarArray(original)
    fmt.Println("após função:", original) // [1 2 3] (não mudou!)

    // Para modificar, passe ponteiro
    modificarArrayPonteiro(&original)
    fmt.Println("após &func:", original) // [100 2 3]
}

func modificarArray(arr [3]int) {
    arr[0] = 999 // modifica apenas a cópia local
}

func modificarArrayPonteiro(arr *[3]int) {
    arr[0] = 100 // modifica o original
}
```

## 9.3 Arrays Multidimensionais

```go
package main

import "fmt"

func main() {
    // Matriz 3x3
    var matriz [3][3]int

    // Preenchendo com valores
    for i := 0; i < 3; i++ {
        for j := 0; j < 3; j++ {
            matriz[i][j] = i*3 + j + 1
        }
    }

    // Imprimindo a matriz
    for _, linha := range matriz {
        fmt.Println(linha)
    }
    // [1 2 3]
    // [4 5 6]
    // [7 8 9]

    // Inicialização literal
    tabuleiro := [3][3]string{
        {"X", "O", "X"},
        {"O", "X", "O"},
        {"X", "O", "X"},
    }
    fmt.Println(tabuleiro)
}
```

---

# 10. Slices

## 10.1 O que são Slices — A Estrutura Interna

Slices são a estrutura de dados mais importante e utilizada em Go. Eles são como "janelas" sobre um array subjacente.

**Internamente, um slice é uma struct com três campos:**

```
Slice Header
+--------+----------+---------+
|  ptr   |  length  |  cap    |
| *array |  (len)   |  (cap)  |
+--------+----------+---------+
    |
    ↓
Array subjacente:
[e0][e1][e2][e3][e4][e5]
```

- `ptr`: ponteiro para o array subjacente
- `len`: número de elementos visíveis
- `cap`: capacidade total do array subjacente a partir de `ptr`

```go
package main

import "fmt"

func main() {
    // Criando um slice com literal
    s := []int{1, 2, 3, 4, 5}

    fmt.Println("slice:", s)
    fmt.Println("len:", len(s)) // 5
    fmt.Println("cap:", cap(s)) // 5

    // Criando slice com make(tipo, len, cap)
    s2 := make([]int, 3, 10)
    fmt.Println("s2:", s2)      // [0 0 0]
    fmt.Println("len:", len(s2)) // 3
    fmt.Println("cap:", cap(s2)) // 10

    // Slice de um array
    arr := [6]int{10, 20, 30, 40, 50, 60}
    sl := arr[1:4] // elementos do índice 1 ao 3 (4 não incluso)
    fmt.Println("sl:", sl)       // [20 30 40]
    fmt.Println("len:", len(sl)) // 3
    fmt.Println("cap:", cap(sl)) // 5 (do índice 1 até o fim do array)

    // IMPORTANTE: modificar o slice modifica o array original!
    sl[0] = 999
    fmt.Println("arr após modificação:", arr) // [10 999 30 40 50 60]
}
```

## 10.2 Operações com Slices

```go
package main

import "fmt"

func main() {
    s := []int{1, 2, 3, 4, 5}

    // Fatiamento (slicing) — sintaxe: s[low:high]
    fmt.Println(s[1:3])  // [2 3] — índices 1 e 2
    fmt.Println(s[:3])   // [1 2 3] — do início ao índice 2
    fmt.Println(s[2:])   // [3 4 5] — do índice 2 até o fim
    fmt.Println(s[:])    // [1 2 3 4 5] — o slice inteiro

    // Slice nil (zero value de slice)
    var nilSlice []int
    fmt.Println(nilSlice == nil) // true
    fmt.Println(len(nilSlice))   // 0
    fmt.Println(cap(nilSlice))   // 0

    // Slice vazio vs nil
    emptySlice := []int{}
    fmt.Println(emptySlice == nil) // false! (não é nil, mas está vazio)
    fmt.Println(len(emptySlice))   // 0

    // Sempre use len() para verificar se está vazio
    if len(nilSlice) == 0 {
        fmt.Println("slice está vazio")
    }
}
```

## 10.3 append — Como Funciona Internamente

```go
package main

import "fmt"

func main() {
    s := []int{1, 2, 3}
    fmt.Printf("antes: len=%d cap=%d %v\n", len(s), cap(s), s)
    // antes: len=3 cap=3 [1 2 3]

    // append adiciona elementos ao final
    s = append(s, 4)
    fmt.Printf("após append(4): len=%d cap=%d %v\n", len(s), cap(s), s)
    // após append(4): len=4 cap=6 [1 2 3 4]
    // NOTA: capacidade dobrou de 3 para 6!

    s = append(s, 5, 6)
    fmt.Printf("após append(5,6): len=%d cap=%d %v\n", len(s), cap(s), s)

    // Quando len == cap, append aloca um novo array maior
    // Regra geral de crescimento (pode variar por versão):
    // - Se cap < 256: dobra
    // - Se cap >= 256: cresce ~25%

    // Demonstrando o crescimento
    fmt.Println("\nCrescimento de capacidade:")
    var growing []int
    lastCap := 0
    for i := 0; i < 20; i++ {
        growing = append(growing, i)
        if cap(growing) != lastCap {
            fmt.Printf("len=%d, cap=%d (realocação!)\n", len(growing), cap(growing))
            lastCap = cap(growing)
        }
    }

    // Append de um slice em outro (operador ...)
    a := []int{1, 2, 3}
    b := []int{4, 5, 6}
    c := append(a, b...)
    fmt.Println("c:", c) // [1 2 3 4 5 6]

    // Removendo elemento do meio do slice
    s2 := []int{1, 2, 3, 4, 5}
    i := 2 // remover índice 2 (valor 3)
    s2 = append(s2[:i], s2[i+1:]...)
    fmt.Println("após remoção:", s2) // [1 2 4 5]
}
```

## 10.4 copy

```go
package main

import "fmt"

func main() {
    src := []int{1, 2, 3, 4, 5}

    // copy faz uma cópia profunda (deep copy) dos dados
    dst := make([]int, len(src))
    n := copy(dst, src)
    fmt.Printf("copiou %d elementos: %v\n", n, dst)
    // copiou 5 elementos: [1 2 3 4 5]

    // Agora modificar dst não afeta src
    dst[0] = 999
    fmt.Println("src:", src) // [1 2 3 4 5] (não mudou!)
    fmt.Println("dst:", dst) // [999 2 3 4 5]

    // copy copia min(len(dst), len(src)) elementos
    pequeno := make([]int, 3)
    copy(pequeno, src)
    fmt.Println("pequeno:", pequeno) // [1 2 3]

    // Copiando parte de um slice
    parte := make([]int, 3)
    copy(parte, src[1:4])
    fmt.Println("parte:", parte) // [2 3 4]

    // Usar copy para inserir elemento no meio
    s := []int{1, 2, 3, 4, 5}
    s = append(s, 0)       // aumenta tamanho
    copy(s[3:], s[2:])     // shift elementos para a direita
    s[2] = 99              // insere no índice 2
    fmt.Println("após inserção:", s) // [1 2 99 3 4 5]
}
```

## 10.5 Slices 2D

```go
package main

import "fmt"

func main() {
    // Slice de slices (não é um array contíguo na memória)
    matriz := [][]int{
        {1, 2, 3},
        {4, 5, 6},
        {7, 8, 9},
    }

    for _, linha := range matriz {
        fmt.Println(linha)
    }

    // Criando dinamicamente
    rows, cols := 3, 4
    grid := make([][]int, rows)
    for i := range grid {
        grid[i] = make([]int, cols)
        for j := range grid[i] {
            grid[i][j] = i*cols + j
        }
    }

    for _, row := range grid {
        fmt.Println(row)
    }
}
```

---

# 11. Maps

## 11.1 Criação e Uso Básico

Maps são tabelas hash — estruturas de dados que mapeiam chaves para valores, com acesso O(1) em média.

```go
package main

import "fmt"

func main() {
    // Criação com make
    idades := make(map[string]int)

    // Atribuição de valores
    idades["Alice"] = 30
    idades["Bob"] = 25
    idades["Carlos"] = 35

    fmt.Println(idades) // map[Alice:30 Bob:25 Carlos:35]

    // Criação com literal
    capitais := map[string]string{
        "Brasil":    "Brasília",
        "Argentina": "Buenos Aires",
        "Chile":     "Santiago",
    }
    fmt.Println(capitais)

    // Leitura de valor
    fmt.Println(capitais["Brasil"]) // Brasília

    // Chave inexistente retorna zero value
    fmt.Println(capitais["Peru"]) // "" (zero value para string)
    fmt.Println(idades["Zara"])   // 0 (zero value para int)

    // Verificação de existência (idioma "comma ok")
    capital, ok := capitais["Peru"]
    if ok {
        fmt.Println("Capital:", capital)
    } else {
        fmt.Println("País não encontrado") // Este será impresso
    }

    // Forma mais comum
    if v, ok := capitais["Brasil"]; ok {
        fmt.Println("Capital do Brasil:", v)
    }

    // Tamanho do map
    fmt.Println("Total de países:", len(capitais)) // 3

    // Atualização de valor
    idades["Alice"] = 31
    fmt.Println("Idade da Alice:", idades["Alice"]) // 31

    // Deleção de chave
    delete(capitais, "Chile")
    fmt.Println("Após deletar Chile:", capitais)

    // Tentar deletar chave inexistente não causa erro
    delete(capitais, "Peru") // sem erro
}
```

## 11.2 Iteração em Maps

```go
package main

import (
    "fmt"
    "sort"
)

func main() {
    precos := map[string]float64{
        "maçã":    2.50,
        "banana":  1.20,
        "laranja": 3.00,
        "uva":     8.50,
    }

    // Iteração com range — ORDEM NÃO É GARANTIDA!
    fmt.Println("Iteração não ordenada:")
    for produto, preco := range precos {
        fmt.Printf("  %s: R$%.2f\n", produto, preco)
    }

    // Para iteração ordenada: extraia as chaves, ordene, itere
    fmt.Println("\nIteração ordenada:")
    chaves := make([]string, 0, len(precos))
    for k := range precos {
        chaves = append(chaves, k)
    }
    sort.Strings(chaves)

    for _, k := range chaves {
        fmt.Printf("  %s: R$%.2f\n", k, precos[k])
    }
}
```

## 11.3 Maps como Conjuntos (Sets)

Go não tem um tipo Set nativo, mas maps podem ser usados para isso:

```go
package main

import "fmt"

func main() {
    // Usando map[T]bool como set
    set := make(map[string]bool)

    // Adicionar elementos
    set["go"] = true
    set["python"] = true
    set["java"] = true

    // Verificar existência
    if set["go"] {
        fmt.Println("go está no set")
    }

    // Remover
    delete(set, "java")

    // Listar elementos
    for item := range set {
        fmt.Println(item)
    }

    // Usando map[T]struct{} é mais eficiente (struct{} não ocupa memória)
    set2 := make(map[string]struct{})
    set2["go"] = struct{}{}
    set2["rust"] = struct{}{}

    if _, ok := set2["go"]; ok {
        fmt.Println("go está no set2")
    }

    // União de dois sets
    s1 := map[string]bool{"a": true, "b": true, "c": true}
    s2 := map[string]bool{"b": true, "c": true, "d": true}

    uniao := make(map[string]bool)
    for k := range s1 {
        uniao[k] = true
    }
    for k := range s2 {
        uniao[k] = true
    }
    fmt.Println("União:", uniao)

    // Interseção
    intersecao := make(map[string]bool)
    for k := range s1 {
        if s2[k] {
            intersecao[k] = true
        }
    }
    fmt.Println("Interseção:", intersecao)
}
```

## 11.4 Maps Aninhados

```go
package main

import "fmt"

func main() {
    // Map de maps
    escola := map[string]map[string]int{
        "Turma A": {
            "Alice": 95,
            "Bob":   87,
        },
        "Turma B": {
            "Carlos": 78,
            "Diana":  92,
        },
    }

    // Acesso
    fmt.Println(escola["Turma A"]["Alice"]) // 95

    // Cuidado: acessar map nil causa panic!
    var turmaC map[string]int
    // turmaC["Eve"] = 90  // PANIC: assignment to entry in nil map

    // Inicialize antes de usar
    escola["Turma C"] = make(map[string]int)
    escola["Turma C"]["Eve"] = 88
    fmt.Println(escola["Turma C"]["Eve"]) // 88
}
```

---

# 12. Funções

## 12.1 Declaração Básica

```go
package main

import "fmt"

// Função simples sem parâmetros e sem retorno
func saudar() {
    fmt.Println("Olá!")
}

// Função com parâmetros
func soma(a int, b int) int {
    return a + b
}

// Parâmetros do mesmo tipo podem ser agrupados
func multiplicar(a, b, c int) int {
    return a * b * c
}

// Múltiplos retornos — característica importante do Go!
func dividir(a, b float64) (float64, error) {
    if b == 0 {
        return 0, fmt.Errorf("divisão por zero: %g / %g", a, b)
    }
    return a / b, nil
}

// Retornos nomeados
func minMax(nums []int) (min, max int) {
    if len(nums) == 0 {
        return 0, 0
    }
    min, max = nums[0], nums[0]
    for _, n := range nums[1:] {
        if n < min {
            min = n
        }
        if n > max {
            max = n
        }
    }
    return // naked return — retorna min e max automaticamente
}

func main() {
    saudar()

    resultado := soma(3, 4)
    fmt.Println("3 + 4 =", resultado)

    fmt.Println("2 * 3 * 4 =", multiplicar(2, 3, 4))

    // Capturando múltiplos retornos
    r, err := dividir(10, 3)
    if err != nil {
        fmt.Println("Erro:", err)
    } else {
        fmt.Printf("10 / 3 = %.4f\n", r)
    }

    // Ignorando retornos com _
    _, err2 := dividir(5, 0)
    if err2 != nil {
        fmt.Println("Erro:", err2)
    }

    // Retornos nomeados
    min, max := minMax([]int{3, 1, 4, 1, 5, 9, 2, 6})
    fmt.Printf("min=%d, max=%d\n", min, max)
}
```

## 12.2 Variadic Functions (Funções Variádicas)

```go
package main

import "fmt"

// ... antes do tipo indica variadic
func somaVariadica(nums ...int) int {
    total := 0
    for _, n := range nums {
        total += n
    }
    return total
}

// Misturando parâmetros normais e variádicos
func log(nivel string, mensagens ...string) {
    fmt.Printf("[%s] ", nivel)
    for i, msg := range mensagens {
        if i > 0 {
            fmt.Print(", ")
        }
        fmt.Print(msg)
    }
    fmt.Println()
}

func main() {
    fmt.Println(somaVariadica(1, 2, 3))         // 6
    fmt.Println(somaVariadica(1, 2, 3, 4, 5))   // 15
    fmt.Println(somaVariadica())                  // 0

    // Passando um slice para função variádica com ...
    numeros := []int{10, 20, 30, 40}
    fmt.Println(somaVariadica(numeros...)) // 100

    log("INFO", "servidor iniciado")
    log("ERROR", "conexão falhou", "tentando reconectar", "timeout")
}
```

## 12.3 Funções como Valores de Primeira Classe

Em Go, funções são cidadãos de primeira classe: podem ser atribuídas a variáveis, passadas como argumentos e retornadas por outras funções.

```go
package main

import (
    "fmt"
    "sort"
)

func main() {
    // Função atribuída a variável
    dobrar := func(x int) int {
        return x * 2
    }
    fmt.Println(dobrar(5)) // 10

    // Passando função como argumento
    numeros := []int{3, 1, 4, 1, 5, 9, 2, 6}
    sort.Slice(numeros, func(i, j int) bool {
        return numeros[i] < numeros[j] // ordem crescente
    })
    fmt.Println(numeros)

    sort.Slice(numeros, func(i, j int) bool {
        return numeros[i] > numeros[j] // ordem decrescente
    })
    fmt.Println(numeros)

    // Higher-order functions
    aplica := func(nums []int, f func(int) int) []int {
        resultado := make([]int, len(nums))
        for i, n := range nums {
            resultado[i] = f(n)
        }
        return resultado
    }

    fmt.Println(aplica([]int{1, 2, 3, 4, 5}, func(x int) int { return x * x }))
    // [1 4 9 16 25]

    fmt.Println(aplica([]int{1, 2, 3, 4, 5}, func(x int) int { return x + 10 }))
    // [11 12 13 14 15]

    // Filtragem funcional
    filtrar := func(nums []int, pred func(int) bool) []int {
        var resultado []int
        for _, n := range nums {
            if pred(n) {
                resultado = append(resultado, n)
            }
        }
        return resultado
    }

    pares := filtrar([]int{1, 2, 3, 4, 5, 6}, func(x int) bool { return x%2 == 0 })
    fmt.Println("pares:", pares) // [2 4 6]
}
```

## 12.4 Closures (Funções Anônimas com Captura)

```go
package main

import "fmt"

// Retornando uma função (closure)
func criarContador() func() int {
    count := 0 // esta variável é capturada pela closure
    return func() int {
        count++
        return count
    }
}

// Closure com parâmetro
func criarSomador(x int) func(int) int {
    return func(y int) int {
        return x + y // x é capturado do escopo externo
    }
}

func main() {
    // Cada chamada a criarContador() cria um novo contexto
    contador1 := criarContador()
    contador2 := criarContador()

    fmt.Println(contador1()) // 1
    fmt.Println(contador1()) // 2
    fmt.Println(contador1()) // 3
    fmt.Println(contador2()) // 1 (independente do contador1!)
    fmt.Println(contador2()) // 2

    // Somadores
    soma5 := criarSomador(5)
    soma10 := criarSomador(10)

    fmt.Println(soma5(3))  // 8
    fmt.Println(soma10(3)) // 13
    fmt.Println(soma5(7))  // 12

    // Cuidado com closures em loops!
    // ERRADO — captura a variável i, não o valor de i
    funcs := make([]func(), 5)
    for i := 0; i < 5; i++ {
        i := i // shadowing — cria uma nova variável i para cada iteração
        funcs[i] = func() {
            fmt.Println(i)
        }
    }
    for _, f := range funcs {
        f()
    }
    // Saída: 0 1 2 3 4 (correto por causa do shadowing)
}
```

## 12.5 defer

`defer` adia a execução de uma função para quando a função que a contém retornar:

```go
package main

import "fmt"

func exemplo1() {
    defer fmt.Println("executado por último")
    fmt.Println("executado primeiro")
    fmt.Println("executado segundo")
}

func exemplo2() {
    // Múltiplos defers são executados em ordem LIFO (pilha)
    for i := 0; i < 5; i++ {
        defer fmt.Println("defer", i)
    }
    fmt.Println("função normal")
}

func lerArquivo(nome string) error {
    // Uso clássico do defer: garantir fechamento de recursos
    // mesmo quando há erro
    fmt.Println("abrindo", nome)

    // Simulando arquivo
    defer func() {
        fmt.Println("fechando", nome)
        // Aqui viria: arquivo.Close()
    }()

    // ... processamento ...
    return nil
}

// defer com recuperação de panic
func seguro() {
    defer func() {
        if r := recover(); r != nil {
            fmt.Println("Recuperado do panic:", r)
        }
    }()

    panic("algo deu muito errado!")
    // O código abaixo não será executado
    fmt.Println("nunca chega aqui")
}

func main() {
    exemplo1()
    fmt.Println("---")
    exemplo2()
    fmt.Println("---")
    lerArquivo("dados.txt")
    fmt.Println("---")
    seguro()
    fmt.Println("Continuando após o panic recuperado")
}
```

---

# 13. Estruturas (Structs)

## 13.1 Criação e Uso Básico

Structs são tipos compostos que agrupam campos relacionados:

```go
package main

import "fmt"

// Definição de struct
type Pessoa struct {
    Nome  string
    Idade int
    Email string
}

// Struct com tipos variados
type Produto struct {
    ID       int
    Nome     string
    Preco    float64
    Estoque  int
    Ativo    bool
    Tags     []string
    Metadado map[string]string
}

func main() {
    // Criando instâncias
    p1 := Pessoa{
        Nome:  "Alice",
        Idade: 30,
        Email: "alice@email.com",
    }

    // Criando sem nomear campos (ordem importa, não recomendado)
    p2 := Pessoa{"Bob", 25, "bob@email.com"}

    // Zero value — todos os campos com seus zero values
    var p3 Pessoa
    fmt.Println(p3) // { 0 }

    // Acessando campos
    fmt.Println(p1.Nome)
    fmt.Println(p1.Idade)
    p1.Email = "newalice@email.com"

    // Ponteiro para struct
    p4 := &Pessoa{Nome: "Carlos", Idade: 28}
    // Go automaticamente dereferencia ponteiros para structs
    p4.Idade = 29 // equivalente a (*p4).Idade = 29
    fmt.Println(p4.Nome, p4.Idade)

    _ = p2
}
```

## 13.2 Métodos em Structs

```go
package main

import (
    "fmt"
    "math"
)

type Circulo struct {
    Raio float64
}

type Retangulo struct {
    Largura float64
    Altura  float64
}

// Método com value receiver (cópia do struct)
func (c Circulo) Area() float64 {
    return math.Pi * c.Raio * c.Raio
}

func (c Circulo) Perimetro() float64 {
    return 2 * math.Pi * c.Raio
}

// Método com pointer receiver (referência ao struct)
// Use quando precisar modificar o struct ou para eficiência com structs grandes
func (c *Circulo) Escalar(fator float64) {
    c.Raio *= fator
}

func (r Retangulo) Area() float64 {
    return r.Largura * r.Altura
}

func (r Retangulo) Perimetro() float64 {
    return 2 * (r.Largura + r.Altura)
}

// String() — se você implementar este método, fmt.Println usa ele
func (c Circulo) String() string {
    return fmt.Sprintf("Circulo(raio=%.2f)", c.Raio)
}

func main() {
    c := Circulo{Raio: 5.0}
    fmt.Println(c)                           // Circulo(raio=5.00)
    fmt.Printf("Área: %.2f\n", c.Area())     // Área: 78.54
    fmt.Printf("Perímetro: %.2f\n", c.Perimetro())

    c.Escalar(2.0) // modifica o raio via pointer receiver
    fmt.Printf("Após escalar: %v\n", c)

    r := Retangulo{Largura: 4, Altura: 6}
    fmt.Printf("Área: %.2f\n", r.Area())
    fmt.Printf("Perímetro: %.2f\n", r.Perimetro())
}
```

## 13.3 Embedding (Composição)

Go usa composição ao invés de herança. O embedding permite que um struct "herde" campos e métodos de outro:

```go
package main

import "fmt"

// Struct base
type Animal struct {
    Nome  string
    Peso  float64
}

func (a Animal) Descrever() string {
    return fmt.Sprintf("%s pesa %.1f kg", a.Nome, a.Peso)
}

func (a Animal) Comer() {
    fmt.Printf("%s está comendo\n", a.Nome)
}

// Embedding: Cachorro "herda" Animal
type Cachorro struct {
    Animal      // campo embutido (embedded)
    Raca string
}

func (c Cachorro) Latir() {
    fmt.Printf("%s: Au au!\n", c.Nome) // acessa Nome diretamente
}

// Override de método
func (c Cachorro) Descrever() string {
    return fmt.Sprintf("%s (%s) pesa %.1f kg", c.Nome, c.Raca, c.Peso)
}

type Gato struct {
    Animal
    PeloLongo bool
}

func (g Gato) Miar() {
    fmt.Printf("%s: Miau!\n", g.Nome)
}

func main() {
    c := Cachorro{
        Animal: Animal{Nome: "Rex", Peso: 25.5},
        Raca:   "Labrador",
    }

    // Acesso direto aos campos do Animal embutido
    fmt.Println(c.Nome)    // Rex (promovido do Animal)
    fmt.Println(c.Peso)    // 25.5
    fmt.Println(c.Raca)    // Labrador

    c.Comer()              // Rex está comendo (método promovido)
    c.Latir()              // Rex: Au au!
    fmt.Println(c.Descrever()) // Rex (Labrador) pesa 25.5 kg (método overridden)

    // Acesso explícito ao Animal embutido
    fmt.Println(c.Animal.Descrever()) // Rex pesa 25.5 kg (método original)

    g := Gato{
        Animal:    Animal{Nome: "Whiskers", Peso: 4.2},
        PeloLongo: true,
    }
    g.Miar()
    g.Comer()
    fmt.Println(g.Descrever()) // método do Animal (não foi overridden)
}
```

## 13.4 Struct Tags

Struct tags são metadados que você pode adicionar aos campos de um struct:

```go
package main

import (
    "encoding/json"
    "fmt"
)

// Tags são usadas por pacotes de reflexão como encoding/json
type Usuario struct {
    ID       int    `json:"id"`
    Nome     string `json:"nome"`
    Email    string `json:"email"`
    Senha    string `json:"-"`          // "-" significa: ignore este campo no JSON
    Apelido  string `json:"apelido,omitempty"` // omit if empty
    Interno  string `json:"interno,omitempty"`
}

func main() {
    u := Usuario{
        ID:    1,
        Nome:  "Alice",
        Email: "alice@email.com",
        Senha: "secret123",
        // Apelido está vazio (não será incluído por omitempty)
    }

    // Serialização para JSON
    jsonData, err := json.MarshalIndent(u, "", "  ")
    if err != nil {
        fmt.Println("Erro:", err)
        return
    }
    fmt.Println(string(jsonData))
    // {
    //   "id": 1,
    //   "nome": "Alice",
    //   "email": "alice@email.com"
    // }
    // Nota: Senha foi ignorada (-), Apelido foi omitido (omitempty + vazio)

    // Desserialização de JSON
    jsonStr := `{"id":2,"nome":"Bob","email":"bob@email.com","apelido":"Bobby"}`
    var u2 Usuario
    json.Unmarshal([]byte(jsonStr), &u2)
    fmt.Printf("%+v\n", u2)
}
```

---

# 14. Interfaces

## 14.1 O Conceito de Interface em Go

Interfaces em Go são fundamentalmente diferentes de outras linguagens. Em Go, **a implementação de uma interface é implícita** — não existe `implements` ou `extends`.

Se um tipo tem todos os métodos que uma interface define, ele automaticamente implementa aquela interface.

```go
package main

import (
    "fmt"
    "math"
)

// Definição de interface
type Forma interface {
    Area() float64
    Perimetro() float64
}

// Circulo implementa Forma (implicitamente, sem declarar)
type Circulo struct {
    Raio float64
}

func (c Circulo) Area() float64 {
    return math.Pi * c.Raio * c.Raio
}

func (c Circulo) Perimetro() float64 {
    return 2 * math.Pi * c.Raio
}

// Retangulo também implementa Forma
type Retangulo struct {
    Largura, Altura float64
}

func (r Retangulo) Area() float64 {
    return r.Largura * r.Altura
}

func (r Retangulo) Perimetro() float64 {
    return 2 * (r.Largura + r.Altura)
}

// Triangulo implementa Forma parcialmente (apenas Area)
// Isso NÃO implementa a interface Forma
type Triangulo struct {
    Base, Altura float64
}

func (t Triangulo) Area() float64 {
    return 0.5 * t.Base * t.Altura
}

// Função que aceita qualquer Forma
func imprimirInfo(f Forma) {
    fmt.Printf("Área: %.2f, Perímetro: %.2f\n", f.Area(), f.Perimetro())
}

func totalArea(formas []Forma) float64 {
    total := 0.0
    for _, f := range formas {
        total += f.Area()
    }
    return total
}

func main() {
    c := Circulo{Raio: 5}
    r := Retangulo{Largura: 4, Altura: 6}

    // Ambos podem ser usados onde Forma é esperado
    imprimirInfo(c)
    imprimirInfo(r)

    // Slice de interfaces
    formas := []Forma{
        Circulo{Raio: 3},
        Retangulo{Largura: 4, Altura: 5},
        Circulo{Raio: 1},
    }

    fmt.Printf("Área total: %.2f\n", totalArea(formas))

    // Triangulo NÃO pode ser usado como Forma
    // t := Triangulo{Base: 3, Altura: 4}
    // imprimirInfo(t)  // ERRO: Triangulo não implementa Forma (Perimetro ausente)
}
```

## 14.2 Interface Vazia (empty interface)

```go
package main

import "fmt"

// interface{} (ou any no Go 1.18+) aceita qualquer tipo
func imprimir(v interface{}) {
    fmt.Printf("tipo: %T, valor: %v\n", v, v)
}

// Função que aceita qualquer tipo (Go 1.18+)
func imprimirModerno(v any) {
    fmt.Printf("tipo: %T, valor: %v\n", v, v)
}

func main() {
    imprimir(42)
    imprimir("hello")
    imprimir(true)
    imprimir([]int{1, 2, 3})
    imprimir(nil)

    // Slice de qualquer coisa
    coisas := []interface{}{42, "hello", true, 3.14, []int{1, 2}}
    for _, c := range coisas {
        imprimir(c)
    }
}
```

## 14.3 Type Assertion e Type Switch

```go
package main

import "fmt"

func processar(v interface{}) {
    // Type assertion: extrai o valor concreto de uma interface
    // Forma segura (com "comma ok"):
    if str, ok := v.(string); ok {
        fmt.Printf("É uma string: %q\n", str)
        return
    }

    if num, ok := v.(int); ok {
        fmt.Printf("É um int: %d (dobro=%d)\n", num, num*2)
        return
    }

    fmt.Printf("Tipo não reconhecido: %T\n", v)
}

// Type switch — mais elegante para múltiplos tipos
func descrever(v interface{}) {
    switch x := v.(type) {
    case nil:
        fmt.Println("nil")
    case int:
        fmt.Printf("int: %d\n", x)
    case float64:
        fmt.Printf("float64: %.2f\n", x)
    case string:
        fmt.Printf("string: %q (len=%d)\n", x, len(x))
    case bool:
        fmt.Printf("bool: %t\n", x)
    case []int:
        fmt.Printf("[]int: %v\n", x)
    default:
        fmt.Printf("desconhecido: %T = %v\n", x, x)
    }
}

func main() {
    processar("hello")
    processar(42)
    processar(3.14)

    fmt.Println("---")
    descrever(nil)
    descrever(42)
    descrever(3.14)
    descrever("go")
    descrever(true)
    descrever([]int{1, 2, 3})
}
```

## 14.4 Interfaces Compostas

```go
package main

import "fmt"

// Interfaces podem ser compostas de outras interfaces
type Ledor interface {
    Ler() string
}

type Escritor interface {
    Escrever(s string)
}

// LedorEscritor combina ambas
type LedorEscritor interface {
    Ledor
    Escritor
}

// Implementação
type Buffer struct {
    dados string
}

func (b *Buffer) Ler() string {
    return b.dados
}

func (b *Buffer) Escrever(s string) {
    b.dados += s
}

func usarLedorEscritor(rw LedorEscritor) {
    rw.Escrever("Olá, ")
    rw.Escrever("Mundo!")
    fmt.Println(rw.Ler())
}

func main() {
    buf := &Buffer{}
    usarLedorEscritor(buf)

    // A interface io.ReadWriter da stdlib é exatamente assim!
    // type ReadWriter interface {
    //     Reader
    //     Writer
    // }
}
```

---

# 15. Ponteiros

## 15.1 O que são Ponteiros

Um ponteiro é uma variável que armazena o **endereço de memória** de outra variável.

```
Memória:
Endereço    Conteúdo
0x1000      42        ← variável x (int)
0x1008      0x1000    ← ponteiro p (aponta para x)
```

```go
package main

import "fmt"

func main() {
    x := 42

    // & obtém o endereço de uma variável
    p := &x
    fmt.Printf("valor de x: %d\n", x)
    fmt.Printf("endereço de x: %p\n", p)   // ex: 0xc000018058
    fmt.Printf("valor de p: %p\n", p)       // mesmo endereço

    // * desreferencia um ponteiro (acessa o valor no endereço)
    fmt.Printf("valor em *p: %d\n", *p)    // 42

    // Modificando o valor através do ponteiro
    *p = 100
    fmt.Printf("x após *p = 100: %d\n", x) // 100! (x foi modificado)

    // Tipo de um ponteiro: *tipo
    var ponteiro *int
    fmt.Println("ponteiro nil:", ponteiro)  // <nil>
    // *ponteiro = 5  // PANIC! não pode derreferenciar nil

    // Verificar antes de usar
    if ponteiro != nil {
        *ponteiro = 5
    }

    // new() aloca memória e retorna ponteiro
    n := new(int)    // *int apontando para um int com zero value
    *n = 99
    fmt.Println("n:", *n) // 99
}
```

## 15.2 Passagem por Valor vs Referência

```go
package main

import "fmt"

// Passagem por valor — a função recebe uma CÓPIA
func dobrarValor(n int) {
    n *= 2
    fmt.Println("dentro da função:", n) // 10
}

// Passagem por referência — a função recebe o ENDEREÇO
func dobrarReferencia(n *int) {
    *n *= 2
    fmt.Println("dentro da função:", *n) // 10
}

type Config struct {
    Debug   bool
    MaxConexoes int
    Prefixo string
}

// Passando struct por valor (cópia)
func ativarDebugValor(c Config) {
    c.Debug = true // modifica apenas a cópia
}

// Passando struct por referência
func ativarDebugRef(c *Config) {
    c.Debug = true // modifica o original
}

func main() {
    n := 5
    dobrarValor(n)
    fmt.Println("após dobrarValor:", n) // 5 (não mudou!)

    dobrarReferencia(&n)
    fmt.Println("após dobrarReferencia:", n) // 10

    c := Config{Debug: false, MaxConexoes: 10}
    ativarDebugValor(c)
    fmt.Println("após ativarDebugValor:", c.Debug) // false (não mudou!)

    ativarDebugRef(&c)
    fmt.Println("após ativarDebugRef:", c.Debug) // true
}
```

## 15.3 Quando Usar Ponteiros

```go
package main

import "fmt"

// Regras gerais:
// 1. Use pointer receiver quando o método modifica o receptor
// 2. Use pointer receiver para tipos grandes (evita cópia)
// 3. Use value receiver quando não precisa modificar e o tipo é pequeno
// 4. Seja consistente: se um método usa pointer, todos devem usar

type Contador struct {
    valor int
}

// Pointer receiver: modifica o struct
func (c *Contador) Incrementar() {
    c.valor++
}

func (c *Contador) Decrementar() {
    c.valor--
}

// Value receiver: só lê o struct
func (c Contador) Valor() int {
    return c.valor
}

func (c Contador) String() string {
    return fmt.Sprintf("Contador(%d)", c.valor)
}

func main() {
    c := Contador{valor: 0}
    c.Incrementar()
    c.Incrementar()
    c.Incrementar()
    c.Decrementar()
    fmt.Println(c.Valor())  // 2
    fmt.Println(c)           // Contador(2)

    // Go auto-endereça quando necessário
    // Se c for um value e o método exige pointer, Go faz &c automaticamente
    c2 := Contador{}
    c2.Incrementar() // Go faz (&c2).Incrementar() automaticamente
    fmt.Println(c2)

    // Mas isso NÃO funciona para valores não endereçáveis:
    // Contador{}.Incrementar()  // ERRO: Contador{} não é endereçável
}
```

---

# 16. Pacotes

## 16.1 Criando e Importando Pacotes

Pacotes são a unidade de modularidade em Go. Todo arquivo `.go` pertence a um pacote.

```
meu_projeto/
├── main.go
├── matematica/
│   ├── operacoes.go
│   └── geometria.go
└── utilitarios/
    └── strings.go
```

`matematica/operacoes.go`:

```go
// O nome do pacote deve ser o nome do diretório (por convenção)
package matematica

import "errors"

// Funções exportadas começam com letra maiúscula
func Somar(a, b float64) float64 {
    return a + b
}

func Subtrair(a, b float64) float64 {
    return a - b
}

func Multiplicar(a, b float64) float64 {
    return a * b
}

func Dividir(a, b float64) (float64, error) {
    if b == 0 {
        return 0, errors.New("divisão por zero")
    }
    return a / b, nil
}

// Funções não exportadas são privadas ao pacote
func validar(n float64) bool {
    return n >= 0
}
```

`matematica/geometria.go`:

```go
package matematica

import "math"

// Área de um círculo
func AreaCirculo(raio float64) float64 {
    return math.Pi * raio * raio
}

// Hipotenusa
func Hipotenusa(a, b float64) float64 {
    return math.Sqrt(a*a + b*b)
}
```

`main.go`:

```go
package main

import (
    "fmt"

    // Importação com caminho relativo ao módulo
    "meu_projeto/matematica"
)

func main() {
    soma := matematica.Somar(3, 4)
    fmt.Println("Soma:", soma)

    area := matematica.AreaCirculo(5)
    fmt.Printf("Área: %.2f\n", area)

    resultado, err := matematica.Dividir(10, 0)
    if err != nil {
        fmt.Println("Erro:", err)
    } else {
        fmt.Println("Divisão:", resultado)
    }
}
```

## 16.2 Aliases e Importações Especiais

```go
package main

import (
    "fmt"

    // Alias para evitar conflito de nomes
    mat "meu_projeto/matematica"

    // Importação com _ (executa apenas o init(), sem usar o pacote)
    _ "image/png" // registra o decoder de PNG

    // Importação com . (importa diretamente no escopo — não recomendado)
    // . "fmt"
)

func main() {
    fmt.Println(mat.Somar(1, 2))
}
```

## 16.3 A Biblioteca Padrão

Go vem com uma biblioteca padrão muito rica. Alguns pacotes importantes:

```go
package main

import (
    "bufio"         // I/O com buffer
    "bytes"         // manipulação de bytes
    "context"       // controle de cancelamento e timeout
    "crypto/sha256" // criptografia
    "encoding/json" // JSON
    "errors"        // criação de erros
    "fmt"           // formatação
    "io"            // interfaces de I/O
    "log"           // logging
    "math"          // funções matemáticas
    "math/rand"     // números aleatórios
    "net/http"      // HTTP
    "os"            // sistema operacional
    "path/filepath" // caminhos de arquivo
    "regexp"        // expressões regulares
    "sort"          // ordenação
    "strconv"       // conversão de strings
    "strings"       // manipulação de strings
    "sync"          // sincronização
    "time"          // tempo e data
    "unicode"       // Unicode
)

func main() {
    // strings
    fmt.Println(strings.ToUpper("golang"))

    // strconv
    n, _ := strconv.Atoi("42")
    fmt.Println(n + 1)

    s := strconv.Itoa(100)
    fmt.Println(s + " items")

    // time
    agora := time.Now()
    fmt.Println(agora.Format("02/01/2006 15:04:05"))

    amanha := agora.Add(24 * time.Hour)
    fmt.Println(amanha.Format("02/01/2006"))

    // math/rand
    rand.Seed(time.Now().UnixNano())
    fmt.Println("Aleatório 0-99:", rand.Intn(100))

    // regexp
    re := regexp.MustCompile(`\d+`)
    fmt.Println(re.FindString("abc123def456")) // 123

    // sha256
    hash := sha256.Sum256([]byte("hello"))
    fmt.Printf("%x\n", hash)

    // Suppress unused import warnings in this example
    _ = bufio.NewReader
    _ = bytes.Buffer{}
    _ = context.Background
    _ = errors.New
    _ = io.EOF
    _ = log.Println
    _ = os.Stdout
    _ = filepath.Join
    _ = sort.Ints
    _ = sync.Mutex{}
    _ = unicode.IsLetter
}
```

---

# 17. Módulos Go

## 17.1 O Sistema de Módulos

O sistema de módulos foi introduzido no Go 1.11 e é obrigatório desde o Go 1.16. Ele resolve o gerenciamento de dependências.

```bash
# Inicializando um módulo
mkdir meu-projeto
cd meu-projeto
go mod init github.com/usuario/meu-projeto

# Isso cria um arquivo go.mod:
# module github.com/usuario/meu-projeto
# 
# go 1.22
```

## 17.2 go.mod e go.sum

O arquivo `go.mod` define o módulo e suas dependências:

```
module github.com/usuario/meu-projeto

go 1.22

require (
    github.com/gin-gonic/gin v1.9.1
    github.com/lib/pq v1.10.9
)

// Substituição local (útil durante desenvolvimento)
replace github.com/usuario/outro-modulo => ../outro-modulo
```

O arquivo `go.sum` contém hashes criptográficos das dependências para verificação de integridade.

## 17.3 Comandos go mod

```bash
# Adicionar dependência
go get github.com/gin-gonic/gin@latest

# Adicionar versão específica
go get github.com/gin-gonic/gin@v1.9.0

# Atualizar todas as dependências
go get -u ./...

# Remover dependências não usadas e baixar novas
go mod tidy

# Baixar todas as dependências (para uso offline)
go mod download

# Listar todas as dependências
go list -m all

# Verificar integridade das dependências
go mod verify

# Criar vendor/ com cópias das dependências
go mod vendor
```

## 17.4 Exemplo Prático com Dependência Externa

```bash
mkdir -p exemplo-modulo
cd exemplo-modulo
go mod init github.com/exemplo/modulo

# Adicionando o pacote de logging zap
go get go.uber.org/zap
```

```go
// main.go
package main

import (
    "go.uber.org/zap"
)

func main() {
    // Criando um logger de produção
    logger, _ := zap.NewProduction()
    defer logger.Sync()

    logger.Info("Servidor iniciado",
        zap.String("versão", "1.0"),
        zap.Int("port", 8080),
    )

    logger.Error("Erro de conexão",
        zap.String("host", "db.example.com"),
        zap.Int("tentativa", 3),
    )
}
```

---

# 18. Manipulação de Arquivos

## 18.1 Leitura de Arquivos

```go
package main

import (
    "bufio"
    "fmt"
    "os"
    "strings"
)

func lerArquivoCompleto(caminho string) (string, error) {
    // os.ReadFile lê o arquivo inteiro de uma vez (simples)
    dados, err := os.ReadFile(caminho)
    if err != nil {
        return "", fmt.Errorf("erro ao ler arquivo: %w", err)
    }
    return string(dados), nil
}

func lerLinhaPorLinha(caminho string) error {
    // Abrir arquivo
    arquivo, err := os.Open(caminho)
    if err != nil {
        return fmt.Errorf("erro ao abrir: %w", err)
    }
    defer arquivo.Close() // SEMPRE feche arquivos!

    // Usar bufio.Scanner para leitura eficiente linha por linha
    scanner := bufio.NewScanner(arquivo)

    numeroLinha := 0
    for scanner.Scan() {
        numeroLinha++
        linha := scanner.Text()
        fmt.Printf("[%d] %s\n", numeroLinha, linha)
    }

    // Verificar erro do scanner
    if err := scanner.Err(); err != nil {
        return fmt.Errorf("erro durante leitura: %w", err)
    }

    return nil
}

func main() {
    // Criando arquivo de teste
    conteudo := "Linha 1\nLinha 2\nLinha 3\n"
    err := os.WriteFile("teste.txt", []byte(conteudo), 0644)
    if err != nil {
        fmt.Println("Erro ao criar arquivo:", err)
        return
    }

    // Lendo o arquivo inteiro
    texto, err := lerArquivoCompleto("teste.txt")
    if err != nil {
        fmt.Println("Erro:", err)
        return
    }
    fmt.Println("Conteúdo completo:")
    fmt.Println(texto)

    // Lendo linha por linha
    fmt.Println("Linha por linha:")
    lerLinhaPorLinha("teste.txt")

    // Limpeza
    os.Remove("teste.txt")
    _ = strings.TrimSpace
}
```

## 18.2 Escrita em Arquivos

```go
package main

import (
    "bufio"
    "fmt"
    "os"
)

func criarArquivo(caminho, conteudo string) error {
    // os.WriteFile: cria ou sobrescreve o arquivo de uma vez
    return os.WriteFile(caminho, []byte(conteudo), 0644)
}

func escreverComBuffer(caminho string) error {
    // Criar/sobrescrever arquivo
    arquivo, err := os.Create(caminho)
    if err != nil {
        return err
    }
    defer arquivo.Close()

    // Usar bufio.Writer para escrever eficientemente
    writer := bufio.NewWriter(arquivo)

    for i := 1; i <= 10; i++ {
        fmt.Fprintf(writer, "Linha %d\n", i)
    }

    // IMPORTANTE: Flush para garantir que dados vão para disco
    return writer.Flush()
}

func adicionarAoArquivo(caminho, conteudo string) error {
    // os.O_APPEND: abrir em modo append
    // os.O_CREATE: criar se não existir
    // os.O_WRONLY: apenas escrita
    arquivo, err := os.OpenFile(caminho, os.O_APPEND|os.O_CREATE|os.O_WRONLY, 0644)
    if err != nil {
        return err
    }
    defer arquivo.Close()

    _, err = fmt.Fprintln(arquivo, conteudo)
    return err
}

func main() {
    // Criar arquivo
    err := criarArquivo("saida.txt", "Primeira linha\n")
    if err != nil {
        fmt.Println("Erro:", err)
        return
    }

    // Adicionar ao arquivo
    for i := 2; i <= 5; i++ {
        adicionarAoArquivo("saida.txt", fmt.Sprintf("Linha %d", i))
    }

    // Ler e imprimir resultado
    dados, _ := os.ReadFile("saida.txt")
    fmt.Println("Conteúdo final:")
    fmt.Println(string(dados))

    // Escrever com buffer
    escreverComBuffer("buffer.txt")
    dados2, _ := os.ReadFile("buffer.txt")
    fmt.Println("Com buffer:")
    fmt.Println(string(dados2))

    // Limpeza
    os.Remove("saida.txt")
    os.Remove("buffer.txt")
}
```

## 18.3 Trabalhando com Diretórios

```go
package main

import (
    "fmt"
    "os"
    "path/filepath"
)

func main() {
    // Criar diretório
    err := os.Mkdir("meu_dir", 0755)
    if err != nil && !os.IsExist(err) {
        fmt.Println("Erro ao criar dir:", err)
        return
    }

    // Criar diretórios aninhados
    os.MkdirAll("pai/filho/neto", 0755)

    // Informações sobre arquivo/diretório
    info, err := os.Stat("meu_dir")
    if err != nil {
        fmt.Println("Erro:", err)
        return
    }
    fmt.Printf("Nome: %s\n", info.Name())
    fmt.Printf("Tamanho: %d bytes\n", info.Size())
    fmt.Printf("É diretório: %t\n", info.IsDir())
    fmt.Printf("Permissões: %s\n", info.Mode())
    fmt.Printf("Modificado em: %s\n", info.ModTime().Format("02/01/2006"))

    // Listar conteúdo de um diretório
    entries, _ := os.ReadDir(".")
    for _, e := range entries {
        tipo := "arquivo"
        if e.IsDir() {
            tipo = "dir"
        }
        fmt.Printf("[%s] %s\n", tipo, e.Name())
    }

    // Caminhar por todos os arquivos (Walk)
    os.WriteFile("meu_dir/arquivo1.txt", []byte("conteúdo"), 0644)
    os.WriteFile("meu_dir/arquivo2.txt", []byte("conteúdo"), 0644)

    fmt.Println("\nTodos os arquivos:")
    filepath.Walk("meu_dir", func(path string, info os.FileInfo, err error) error {
        if err != nil {
            return err
        }
        if !info.IsDir() {
            fmt.Printf("  %s (%d bytes)\n", path, info.Size())
        }
        return nil
    })

    // Limpeza
    os.RemoveAll("meu_dir")
    os.RemoveAll("pai")
}
```

---

# 19. Tratamento de Erros

## 19.1 A Filosofia de Erros em Go

Go trata erros como **valores normais**, não como exceções. Isso é uma das características mais controversas e também mais impactantes da linguagem.

```go
package main

import (
    "errors"
    "fmt"
)

// error é uma interface da biblioteca padrão:
// type error interface {
//     Error() string
// }

// Criando erros simples
var ErrNaoEncontrado = errors.New("registro não encontrado")
var ErrPermissaoNegada = errors.New("permissão negada")

// Função que retorna erro
func buscarUsuario(id int) (string, error) {
    usuarios := map[int]string{
        1: "Alice",
        2: "Bob",
    }

    if nome, ok := usuarios[id]; ok {
        return nome, nil
    }
    return "", ErrNaoEncontrado
}

func main() {
    // Forma idiomática de tratar erros em Go
    nome, err := buscarUsuario(1)
    if err != nil {
        fmt.Println("Erro:", err)
        return
    }
    fmt.Println("Usuário:", nome)

    _, err = buscarUsuario(99)
    if err != nil {
        // Comparando erros com sentinel values
        if errors.Is(err, ErrNaoEncontrado) {
            fmt.Println("O usuário não existe")
        } else {
            fmt.Println("Erro inesperado:", err)
        }
    }
}
```

## 19.2 Erros Personalizados

```go
package main

import (
    "errors"
    "fmt"
)

// Erro personalizado implementando a interface error
type ErroValidacao struct {
    Campo   string
    Mensagem string
}

func (e *ErroValidacao) Error() string {
    return fmt.Sprintf("validação falhou no campo '%s': %s", e.Campo, e.Mensagem)
}

// Erro com código de status HTTP
type ErroHTTP struct {
    Codigo    int
    Mensagem  string
    Cause     error
}

func (e *ErroHTTP) Error() string {
    if e.Cause != nil {
        return fmt.Sprintf("HTTP %d: %s (causa: %v)", e.Codigo, e.Mensagem, e.Cause)
    }
    return fmt.Sprintf("HTTP %d: %s", e.Codigo, e.Mensagem)
}

// Unwrap permite encadeamento de erros
func (e *ErroHTTP) Unwrap() error {
    return e.Cause
}

func validarEmail(email string) error {
    if len(email) < 5 {
        return &ErroValidacao{Campo: "email", Mensagem: "muito curto"}
    }
    return nil
}

func buscarDados(id int) error {
    cause := fmt.Errorf("timeout na conexão com o banco")
    return &ErroHTTP{Codigo: 503, Mensagem: "Serviço indisponível", Cause: cause}
}

func main() {
    err := validarEmail("a@b")
    if err != nil {
        // Extraindo o tipo específico do erro
        var erroVal *ErroValidacao
        if errors.As(err, &erroVal) {
            fmt.Printf("Campo: %s\n", erroVal.Campo)
            fmt.Printf("Mensagem: %s\n", erroVal.Mensagem)
        }
    }

    err2 := buscarDados(1)
    if err2 != nil {
        fmt.Println("Erro:", err2)

        var erroHTTP *ErroHTTP
        if errors.As(err2, &erroHTTP) {
            fmt.Println("Código HTTP:", erroHTTP.Codigo)
            fmt.Println("Causa:", erroHTTP.Cause)
        }
    }
}
```

## 19.3 Wrapping de Erros com %w

```go
package main

import (
    "errors"
    "fmt"
)

var ErrBancoDados = errors.New("erro de banco de dados")

func consultarDB(query string) error {
    // Simulando um erro de banco
    return fmt.Errorf("falha ao executar query '%s': %w", query, ErrBancoDados)
}

func buscarProduto(id int) error {
    err := consultarDB(fmt.Sprintf("SELECT * FROM produtos WHERE id = %d", id))
    if err != nil {
        // Wrapping adiciona contexto sem perder o erro original
        return fmt.Errorf("buscarProduto(%d): %w", id, err)
    }
    return nil
}

func main() {
    err := buscarProduto(42)
    if err != nil {
        fmt.Println("Erro:", err)
        // Saída: buscarProduto(42): falha ao executar query 'SELECT...': erro de banco de dados

        // errors.Is percorre a cadeia de erros wrappados
        if errors.Is(err, ErrBancoDados) {
            fmt.Println("Confirmado: é um erro de banco de dados")
        }

        // Unwrap manualmente
        fmt.Println("\nCadeia de erros:")
        for e := err; e != nil; e = errors.Unwrap(e) {
            fmt.Printf("  - %s\n", e)
        }
    }
}
```

## 19.4 panic e recover

```go
package main

import "fmt"

// panic: lança uma exceção não tratável (use com MUITO cuidado)
// recover: captura um panic (use apenas em defers)

func dividirOuPanicar(a, b int) int {
    if b == 0 {
        panic("divisão por zero: isso é catastrófico!")
    }
    return a / b
}

// Wrapper seguro que transforma panic em error
func dividirSeguro(a, b int) (resultado int, err error) {
    defer func() {
        if r := recover(); r != nil {
            err = fmt.Errorf("panic recuperado: %v", r)
        }
    }()

    resultado = dividirOuPanicar(a, b)
    return
}

func main() {
    // Usando versão segura
    r, err := dividirSeguro(10, 2)
    fmt.Println(r, err) // 5 <nil>

    r2, err2 := dividirSeguro(10, 0)
    fmt.Println(r2, err2) // 0 panic recuperado: divisão por zero: ...

    // Quando usar panic:
    // 1. Erros de programação (bugs) que nunca deveriam acontecer
    // 2. Falhas de inicialização crítica
    // Quando NÃO usar panic:
    // - Para tratar erros normais de runtime
    // - Para erros que podem ser recuperáveis
}
```

---

# 20. Concorrência — Goroutines e Channels

## 20.1 O Modelo de Concorrência do Go

Go usa um modelo de concorrência baseado em **CSP (Communicating Sequential Processes)**, popularizado por Tony Hoare em 1978.

O motto do Go para concorrência é:

> **"Don't communicate by sharing memory; share memory by communicating."** — Rob Pike

```
Modelo tradicional (threads compartilhando memória):
Thread 1 ─────────────┐
                       ↓
                  Memória Compartilhada (com mutex)
                       ↑
Thread 2 ─────────────┘

Modelo Go (goroutines com channels):
Goroutine 1 ──[dado]──→ Channel ──[dado]──→ Goroutine 2
```

## 20.2 Goroutines

Uma goroutine é uma thread leve gerenciada pelo runtime do Go. É muito mais barata que uma thread do SO: começa com ~2KB de stack (vs ~2MB de uma thread).

```go
package main

import (
    "fmt"
    "time"
)

func tarefa(id int) {
    for i := 0; i < 3; i++ {
        fmt.Printf("Goroutine %d: passo %d\n", id, i)
        time.Sleep(100 * time.Millisecond)
    }
}

func main() {
    // Execução sequencial (sem goroutines)
    fmt.Println("=== Sequencial ===")
    tarefa(1)
    tarefa(2)

    // Execução concorrente com goroutines
    fmt.Println("\n=== Concorrente ===")
    go tarefa(3) // executa tarefa(3) em uma goroutine separada
    go tarefa(4)

    // PROBLEMA: main pode terminar antes das goroutines
    // Precisamos esperar — veremos WaitGroup depois
    time.Sleep(500 * time.Millisecond)
    fmt.Println("main terminando")
}
```

### Como goroutines funcionam internamente

```
Runtime Go tem um scheduler M:N (múltiplas goroutines em múltiplas threads)

P (Processor) — contexto de execução
M (Machine) — thread do SO
G (Goroutine) — goroutine

  M1 (thread OS)    M2 (thread OS)
    |                  |
    P1                 P2
   /|\               /|\
  G G G             G G G    ← Local Run Queue
  
Global Run Queue (goroutines esperando um P)
  G G G G G G G G G G
```

O scheduler Go implementa **work-stealing**: quando um P fica sem trabalho, ele rouba goroutines da fila de outro P.

## 20.3 Channels (Canais)

Channels são o mecanismo de comunicação entre goroutines:

```go
package main

import "fmt"

func main() {
    // Criando um channel não-bufferizado
    // send e receive são sincronizados (bloqueiam até o outro lado estar pronto)
    ch := make(chan int)

    // Enviando em uma goroutine
    go func() {
        fmt.Println("enviando 42...")
        ch <- 42 // bloqueia até alguém receber
        fmt.Println("enviado!")
    }()

    // Recebendo no main
    valor := <-ch // bloqueia até alguém enviar
    fmt.Println("recebido:", valor)

    // Channel com direção (mais seguro)
    var soEnvio chan<- int  // só pode enviar
    var soRecebe <-chan int // só pode receber
    _ = soEnvio
    _ = soRecebe
}
```

### Channels Bufferizados

```go
package main

import "fmt"

func main() {
    // Channel bufferizado: não bloqueia até o buffer encher
    ch := make(chan string, 3)

    // Podemos enviar até 3 valores sem bloquear
    ch <- "primeiro"
    ch <- "segundo"
    ch <- "terceiro"
    // ch <- "quarto"  // DEADLOCK! buffer cheio

    // Recebendo valores
    fmt.Println(<-ch) // primeiro
    fmt.Println(<-ch) // segundo
    fmt.Println(<-ch) // terceiro

    // Verificando estado do channel
    fmt.Println("len:", len(ch))  // elementos no buffer
    fmt.Println("cap:", cap(ch))  // capacidade do buffer

    // Channel com comma-ok (verificar se está fechado)
    ch2 := make(chan int, 2)
    ch2 <- 10
    close(ch2)

    v1, ok1 := <-ch2
    fmt.Println(v1, ok1) // 10 true

    v2, ok2 := <-ch2
    fmt.Println(v2, ok2) // 0 false (channel fechado e vazio)
}
```

### Padrão Producer-Consumer

```go
package main

import (
    "fmt"
    "sync"
)

func produtor(ch chan<- int, wg *sync.WaitGroup) {
    defer wg.Done()
    defer close(ch) // fecha o channel quando o produtor terminar

    for i := 0; i < 10; i++ {
        ch <- i
        fmt.Printf("Produziu: %d\n", i)
    }
}

func consumidor(id int, ch <-chan int, wg *sync.WaitGroup) {
    defer wg.Done()

    // range em channel recebe valores até o channel ser fechado
    for v := range ch {
        fmt.Printf("Consumidor %d recebeu: %d\n", id, v)
    }
}

func main() {
    ch := make(chan int, 5)
    var wg sync.WaitGroup

    wg.Add(1)
    go produtor(ch, &wg)

    // Múltiplos consumidores
    for i := 1; i <= 3; i++ {
        wg.Add(1)
        go consumidor(i, ch, &wg)
    }

    wg.Wait()
    fmt.Println("Tudo processado!")
}
```

## 20.4 select — Multiplexando Channels

`select` permite esperar em múltiplos channels simultaneamente:

```go
package main

import (
    "fmt"
    "time"
)

func main() {
    ch1 := make(chan string)
    ch2 := make(chan string)

    go func() {
        time.Sleep(100 * time.Millisecond)
        ch1 <- "resultado do ch1"
    }()

    go func() {
        time.Sleep(200 * time.Millisecond)
        ch2 <- "resultado do ch2"
    }()

    // select espera pelo primeiro channel que tiver dados
    for i := 0; i < 2; i++ {
        select {
        case msg1 := <-ch1:
            fmt.Println("ch1:", msg1)
        case msg2 := <-ch2:
            fmt.Println("ch2:", msg2)
        }
    }

    // select com timeout usando time.After
    ch3 := make(chan int)
    go func() {
        time.Sleep(2 * time.Second)
        ch3 <- 42
    }()

    select {
    case v := <-ch3:
        fmt.Println("Recebido:", v)
    case <-time.After(500 * time.Millisecond):
        fmt.Println("Timeout! Operação demorou demais.")
    }

    // select com default (não bloqueante)
    ch4 := make(chan int)
    select {
    case v := <-ch4:
        fmt.Println("Recebido:", v)
    default:
        fmt.Println("Nenhum dado disponível (não-bloqueante)")
    }
}
```

---

# 21. Goroutines Avançadas

## 21.1 Worker Pool

O padrão Worker Pool distribui trabalho entre múltiplos workers:

```go
package main

import (
    "fmt"
    "sync"
    "time"
)

type Tarefa struct {
    ID    int
    Dados string
}

type Resultado struct {
    TarefaID int
    Saida    string
    Erro     error
}

func worker(id int, tarefas <-chan Tarefa, resultados chan<- Resultado, wg *sync.WaitGroup) {
    defer wg.Done()

    for tarefa := range tarefas {
        // Simula processamento
        time.Sleep(50 * time.Millisecond)
        saida := fmt.Sprintf("Worker %d processou tarefa %d: %s→FEITO", id, tarefa.ID, tarefa.Dados)

        resultados <- Resultado{
            TarefaID: tarefa.ID,
            Saida:    saida,
        }
    }
}

func main() {
    const numWorkers = 3
    const numTarefas = 10

    tarefas := make(chan Tarefa, numTarefas)
    resultados := make(chan Resultado, numTarefas)

    var wg sync.WaitGroup

    // Iniciar workers
    for i := 1; i <= numWorkers; i++ {
        wg.Add(1)
        go worker(i, tarefas, resultados, &wg)
    }

    // Enviar tarefas
    for i := 1; i <= numTarefas; i++ {
        tarefas <- Tarefa{ID: i, Dados: fmt.Sprintf("dados-%d", i)}
    }
    close(tarefas) // sinaliza que não há mais tarefas

    // Goroutine para fechar resultados quando todos workers terminarem
    go func() {
        wg.Wait()
        close(resultados)
    }()

    // Coletar resultados
    for r := range resultados {
        if r.Erro != nil {
            fmt.Printf("Erro na tarefa %d: %v\n", r.TarefaID, r.Erro)
        } else {
            fmt.Println(r.Saida)
        }
    }
}
```

## 21.2 Pipeline

O padrão Pipeline encadeia goroutines onde a saída de uma é a entrada da próxima:

```go
package main

import (
    "fmt"
    "math"
)

// Estágio 1: Gerar números
func gerarNumeros(numeros ...int) <-chan int {
    out := make(chan int)
    go func() {
        defer close(out)
        for _, n := range numeros {
            out <- n
        }
    }()
    return out
}

// Estágio 2: Calcular quadrado
func calcularQuadrado(in <-chan int) <-chan float64 {
    out := make(chan float64)
    go func() {
        defer close(out)
        for n := range in {
            out <- math.Pow(float64(n), 2)
        }
    }()
    return out
}

// Estágio 3: Calcular raiz quadrada
func calcularRaiz(in <-chan float64) <-chan float64 {
    out := make(chan float64)
    go func() {
        defer close(out)
        for n := range in {
            out <- math.Sqrt(n)
        }
    }()
    return out
}

// Estágio 4: Filtrar apenas valores > 3
func filtrar(in <-chan float64, minimo float64) <-chan float64 {
    out := make(chan float64)
    go func() {
        defer close(out)
        for n := range in {
            if n > minimo {
                out <- n
            }
        }
    }()
    return out
}

func main() {
    // Pipeline: gerar → quadrado → raiz → filtrar
    // (quadrar e tirar raiz retorna o número original, mas ilustra o padrão)
    numeros := gerarNumeros(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
    quadrados := calcularQuadrado(numeros)
    raizes := calcularRaiz(quadrados)
    filtrados := filtrar(raizes, 3.0)

    for resultado := range filtrados {
        fmt.Printf("%.2f\n", resultado)
    }
}
```

## 21.3 Context para Cancelamento

```go
package main

import (
    "context"
    "fmt"
    "time"
)

func operacaoLonga(ctx context.Context, id int) error {
    select {
    case <-time.After(2 * time.Second):
        fmt.Printf("Operação %d concluída\n", id)
        return nil
    case <-ctx.Done():
        fmt.Printf("Operação %d cancelada: %v\n", id, ctx.Err())
        return ctx.Err()
    }
}

func main() {
    // Context com timeout
    ctx, cancel := context.WithTimeout(context.Background(), 500*time.Millisecond)
    defer cancel()

    err := operacaoLonga(ctx, 1)
    if err != nil {
        fmt.Println("Erro:", err)
    }

    // Context com cancelamento manual
    ctx2, cancel2 := context.WithCancel(context.Background())

    go func() {
        time.Sleep(100 * time.Millisecond)
        fmt.Println("Cancelando operações...")
        cancel2()
    }()

    err2 := operacaoLonga(ctx2, 2)
    if err2 != nil {
        fmt.Println("Erro:", err2)
    }

    // Context com valor (passando dados pelo contexto)
    type chaveContexto string
    const chaveUsuario chaveContexto = "usuario"

    ctx3 := context.WithValue(context.Background(), chaveUsuario, "Alice")

    processarComUsuario := func(ctx context.Context) {
        usuario := ctx.Value(chaveUsuario).(string)
        fmt.Printf("Processando para: %s\n", usuario)
    }
    processarComUsuario(ctx3)
}
```

---

# 22. Mutex e Sincronização

## 22.1 Race Conditions

```go
package main

import (
    "fmt"
    "sync"
)

// PROBLEMA: race condition sem mutex
type ContadorInseguro struct {
    valor int
}

func (c *ContadorInseguro) Incrementar() {
    c.valor++ // NÃO É THREAD-SAFE!
}

// SOLUÇÃO: usando sync.Mutex
type ContadorSeguro struct {
    mu    sync.Mutex
    valor int
}

func (c *ContadorSeguro) Incrementar() {
    c.mu.Lock()         // adquire o lock
    defer c.mu.Unlock() // libera o lock ao sair da função
    c.valor++
}

func (c *ContadorSeguro) Valor() int {
    c.mu.Lock()
    defer c.mu.Unlock()
    return c.valor
}

func main() {
    const numGoroutines = 1000
    var wg sync.WaitGroup

    // Contador INSEGURO — resultado imprevisível
    inseguro := &ContadorInseguro{}
    wg.Add(numGoroutines)
    for i := 0; i < numGoroutines; i++ {
        go func() {
            defer wg.Done()
            inseguro.Incrementar()
        }()
    }
    wg.Wait()
    fmt.Printf("Inseguro: esperado=%d, obtido=%d\n", numGoroutines, inseguro.valor)
    // Provavelmente != 1000 por causa da race condition

    // Contador SEGURO — resultado sempre correto
    seguro := &ContadorSeguro{}
    wg.Add(numGoroutines)
    for i := 0; i < numGoroutines; i++ {
        go func() {
            defer wg.Done()
            seguro.Incrementar()
        }()
    }
    wg.Wait()
    fmt.Printf("Seguro: esperado=%d, obtido=%d\n", numGoroutines, seguro.Valor())
    // Sempre = 1000
}
```

### Detectando Race Conditions

```bash
# O Go tem um detector de race conditions embutido!
go run -race main.go
go test -race ./...
```

## 22.2 sync.RWMutex

Para cenários com muitas leituras e poucas escritas, `RWMutex` é mais eficiente:

```go
package main

import (
    "fmt"
    "sync"
    "time"
)

type Cache struct {
    mu    sync.RWMutex
    dados map[string]string
}

func (c *Cache) Set(chave, valor string) {
    c.mu.Lock()         // lock exclusivo para escrita
    defer c.mu.Unlock()
    c.dados[chave] = valor
}

func (c *Cache) Get(chave string) (string, bool) {
    c.mu.RLock()         // lock compartilhado para leitura
    defer c.mu.RUnlock() // múltiplas goroutines podem ler simultaneamente!
    v, ok := c.dados[chave]
    return v, ok
}

func NewCache() *Cache {
    return &Cache{dados: make(map[string]string)}
}

func main() {
    cache := NewCache()
    var wg sync.WaitGroup

    // Escritores (poucos)
    for i := 0; i < 3; i++ {
        wg.Add(1)
        i := i
        go func() {
            defer wg.Done()
            chave := fmt.Sprintf("chave%d", i)
            cache.Set(chave, fmt.Sprintf("valor%d", i))
            fmt.Printf("Escreveu: %s\n", chave)
        }()
    }

    // Leitores (muitos)
    for i := 0; i < 10; i++ {
        wg.Add(1)
        i := i
        go func() {
            defer wg.Done()
            time.Sleep(10 * time.Millisecond)
            chave := fmt.Sprintf("chave%d", i%3)
            v, ok := cache.Get(chave)
            if ok {
                fmt.Printf("Leu: %s=%s\n", chave, v)
            }
        }()
    }

    wg.Wait()
}
```

## 22.3 sync.WaitGroup

```go
package main

import (
    "fmt"
    "sync"
    "time"
)

func downloadArquivo(url string, wg *sync.WaitGroup) {
    defer wg.Done() // SEMPRE chame Done, mesmo em caso de erro

    // Simulando download
    time.Sleep(100 * time.Millisecond)
    fmt.Printf("Download completo: %s\n", url)
}

func main() {
    urls := []string{
        "https://exemplo.com/arquivo1.zip",
        "https://exemplo.com/arquivo2.zip",
        "https://exemplo.com/arquivo3.zip",
        "https://exemplo.com/arquivo4.zip",
    }

    var wg sync.WaitGroup

    for _, url := range urls {
        wg.Add(1)          // incrementa ANTES de iniciar a goroutine
        url := url         // shadowing necessário para closures em loops
        go downloadArquivo(url, &wg)
    }

    wg.Wait() // bloqueia até todos chamarem Done()
    fmt.Println("Todos os downloads concluídos!")
}
```

## 22.4 sync.Once

```go
package main

import (
    "fmt"
    "sync"
)

// Singleton com Once
type Database struct {
    conexao string
}

var (
    instance *Database
    once     sync.Once
)

func GetDatabase() *Database {
    once.Do(func() {
        // Executado apenas UMA VEZ, mesmo com múltiplas goroutines
        fmt.Println("Inicializando banco de dados...")
        instance = &Database{conexao: "postgresql://localhost/mydb"}
    })
    return instance
}

func main() {
    var wg sync.WaitGroup

    for i := 0; i < 5; i++ {
        wg.Add(1)
        go func(id int) {
            defer wg.Done()
            db := GetDatabase()
            fmt.Printf("Goroutine %d: usando %s\n", id, db.conexao)
        }(i)
    }

    wg.Wait()
    // "Inicializando banco de dados..." aparece apenas UMA VEZ
}
```

## 22.5 sync.Map

```go
package main

import (
    "fmt"
    "sync"
)

func main() {
    var m sync.Map

    // Armazenar valor
    m.Store("chave1", "valor1")
    m.Store("chave2", 42)
    m.Store("chave3", []int{1, 2, 3})

    // Carregar valor
    if v, ok := m.Load("chave1"); ok {
        fmt.Println("chave1:", v)
    }

    // LoadOrStore: carrega se existe, armazena se não existe
    v, loaded := m.LoadOrStore("chave1", "novo_valor")
    fmt.Printf("loaded=%t, valor=%v\n", loaded, v)

    v2, loaded2 := m.LoadOrStore("chave4", "novo")
    fmt.Printf("loaded=%t, valor=%v\n", loaded2, v2)

    // Deletar
    m.Delete("chave2")

    // Iterar (Range)
    m.Range(func(k, v interface{}) bool {
        fmt.Printf("  %v: %v\n", k, v)
        return true // retornar false para parar a iteração
    })
}
```

---

# 23. JSON em Go

## 23.1 Marshaling (Go → JSON)

```go
package main

import (
    "encoding/json"
    "fmt"
)

type Endereco struct {
    Rua    string `json:"rua"`
    Cidade string `json:"cidade"`
    Estado string `json:"estado"`
    CEP    string `json:"cep"`
}

type Pessoa struct {
    ID       int      `json:"id"`
    Nome     string   `json:"nome"`
    Email    string   `json:"email"`
    Idade    int      `json:"idade"`
    Endereco Endereco `json:"endereco"`
    Hobbies  []string `json:"hobbies"`
    Ativo    bool     `json:"ativo"`
    // Tags especiais:
    Senha    string  `json:"-"`              // ignorar
    Apelido  string  `json:"apelido,omitempty"` // omitir se vazio
    Score    float64 `json:"score,omitempty"`
}

func main() {
    p := Pessoa{
        ID:    1,
        Nome:  "Alice",
        Email: "alice@email.com",
        Idade: 30,
        Endereco: Endereco{
            Rua:    "Rua das Flores, 123",
            Cidade: "São Paulo",
            Estado: "SP",
            CEP:    "01234-567",
        },
        Hobbies: []string{"leitura", "programação", "ciclismo"},
        Ativo:   true,
        Senha:   "super_secret", // será ignorada no JSON
    }

    // Marshal: struct → JSON bytes
    jsonBytes, err := json.Marshal(p)
    if err != nil {
        fmt.Println("Erro:", err)
        return
    }
    fmt.Println("Compacto:", string(jsonBytes))

    // MarshalIndent: JSON formatado
    jsonBonito, _ := json.MarshalIndent(p, "", "  ")
    fmt.Println("\nFormatado:")
    fmt.Println(string(jsonBonito))

    // Slice de structs
    pessoas := []Pessoa{
        {ID: 1, Nome: "Alice", Email: "alice@email.com"},
        {ID: 2, Nome: "Bob", Email: "bob@email.com"},
    }
    jsonPessoas, _ := json.MarshalIndent(pessoas, "", "  ")
    fmt.Println("\nLista:")
    fmt.Println(string(jsonPessoas))
}
```

## 23.2 Unmarshaling (JSON → Go)

```go
package main

import (
    "encoding/json"
    "fmt"
)

type Produto struct {
    ID       int      `json:"id"`
    Nome     string   `json:"nome"`
    Preco    float64  `json:"preco"`
    Tags     []string `json:"tags"`
    Estoque  *int     `json:"estoque"` // ponteiro para distinguir 0 de ausente
}

func main() {
    // JSON simples
    jsonStr := `{
        "id": 1,
        "nome": "Notebook Go",
        "preco": 2999.99,
        "tags": ["eletrônico", "computador"],
        "estoque": 15
    }`

    var produto Produto
    err := json.Unmarshal([]byte(jsonStr), &produto)
    if err != nil {
        fmt.Println("Erro:", err)
        return
    }
    fmt.Printf("Produto: %+v\n", produto)
    if produto.Estoque != nil {
        fmt.Println("Estoque:", *produto.Estoque)
    }

    // JSON sem o campo "estoque"
    jsonSemEstoque := `{"id": 2, "nome": "Teclado", "preco": 199.90}`
    var p2 Produto
    json.Unmarshal([]byte(jsonSemEstoque), &p2)
    fmt.Println("Estoque é nil:", p2.Estoque == nil) // true

    // Array JSON
    jsonArray := `[
        {"id": 1, "nome": "Item A", "preco": 10.0},
        {"id": 2, "nome": "Item B", "preco": 20.0}
    ]`
    var produtos []Produto
    json.Unmarshal([]byte(jsonArray), &produtos)
    for _, p := range produtos {
        fmt.Printf("  %d: %s - R$%.2f\n", p.ID, p.Nome, p.Preco)
    }

    // JSON para map (quando a estrutura é desconhecida)
    jsonGenerico := `{"nome": "Alice", "idade": 30, "ativo": true}`
    var dados map[string]interface{}
    json.Unmarshal([]byte(jsonGenerico), &dados)
    fmt.Println("nome:", dados["nome"])
    fmt.Println("idade:", dados["idade"])
}
```

## 23.3 Encoder e Decoder (para Streams)

```go
package main

import (
    "bytes"
    "encoding/json"
    "fmt"
    "strings"
)

type Mensagem struct {
    Tipo    string `json:"tipo"`
    Conteudo string `json:"conteudo"`
}

func main() {
    // Encoder: escreve JSON em um io.Writer
    var buf bytes.Buffer
    encoder := json.NewEncoder(&buf)
    encoder.SetIndent("", "  ")

    mensagens := []Mensagem{
        {Tipo: "chat", Conteudo: "Olá!"},
        {Tipo: "sistema", Conteudo: "Usuário entrou"},
    }

    for _, msg := range mensagens {
        encoder.Encode(msg) // adiciona \n após cada objeto
    }

    fmt.Println("Encoded:")
    fmt.Println(buf.String())

    // Decoder: lê JSON de um io.Reader
    jsonStream := `{"tipo":"a","conteudo":"um"}
{"tipo":"b","conteudo":"dois"}
{"tipo":"c","conteudo":"três"}`

    decoder := json.NewDecoder(strings.NewReader(jsonStream))

    fmt.Println("Decoded:")
    for decoder.More() {
        var msg Mensagem
        if err := decoder.Decode(&msg); err != nil {
            fmt.Println("Erro:", err)
            break
        }
        fmt.Printf("  tipo=%s, conteudo=%s\n", msg.Tipo, msg.Conteudo)
    }
}
```

---

# 24. HTTP em Go

## 24.1 Servidor HTTP Básico

```go
package main

import (
    "fmt"
    "log"
    "net/http"
    "time"
)

// Handler como função
func handlerOla(w http.ResponseWriter, r *http.Request) {
    // w: ResponseWriter — onde escrever a resposta
    // r: *Request — informações sobre a requisição

    nome := r.URL.Query().Get("nome")
    if nome == "" {
        nome = "Mundo"
    }
    fmt.Fprintf(w, "Olá, %s!", nome)
}

func handlerInfo(w http.ResponseWriter, r *http.Request) {
    fmt.Fprintf(w, "Método: %s\n", r.Method)
    fmt.Fprintf(w, "URL: %s\n", r.URL.Path)
    fmt.Fprintf(w, "Host: %s\n", r.Host)
    fmt.Fprintf(w, "IP: %s\n", r.RemoteAddr)
    fmt.Fprintf(w, "User-Agent: %s\n", r.UserAgent())

    for k, v := range r.Header {
        fmt.Fprintf(w, "Header %s: %v\n", k, v)
    }
}

// Middleware de logging
func middlewareLog(proximo http.Handler) http.Handler {
    return http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
        inicio := time.Now()
        proximo.ServeHTTP(w, r)
        log.Printf("%s %s %v", r.Method, r.URL.Path, time.Since(inicio))
    })
}

func main() {
    mux := http.NewServeMux()

    // Registrar rotas
    mux.HandleFunc("/", func(w http.ResponseWriter, r *http.Request) {
        fmt.Fprintln(w, "Bem-vindo ao servidor Go!")
    })
    mux.HandleFunc("/ola", handlerOla)
    mux.HandleFunc("/info", handlerInfo)

    // Handler com tipo
    mux.Handle("/estático/", http.StripPrefix("/estático/", http.FileServer(http.Dir("."))))

    // Servidor com configurações
    servidor := &http.Server{
        Addr:         ":8080",
        Handler:      middlewareLog(mux),
        ReadTimeout:  15 * time.Second,
        WriteTimeout: 15 * time.Second,
        IdleTimeout:  60 * time.Second,
    }

    fmt.Println("Servidor iniciado em http://localhost:8080")
    log.Fatal(servidor.ListenAndServe())
}
```

## 24.2 API REST Completa

```go
package main

import (
    "encoding/json"
    "fmt"
    "log"
    "net/http"
    "strconv"
    "strings"
    "sync"
    "time"
)

// Modelo
type Tarefa struct {
    ID        int       `json:"id"`
    Titulo    string    `json:"titulo"`
    Feita     bool      `json:"feita"`
    CriadaEm time.Time `json:"criada_em"`
}

// "Banco de dados" em memória
type TarefaStore struct {
    mu      sync.RWMutex
    tarefas map[int]*Tarefa
    nextID  int
}

func NewTarefaStore() *TarefaStore {
    return &TarefaStore{
        tarefas: make(map[int]*Tarefa),
        nextID:  1,
    }
}

func (s *TarefaStore) Criar(titulo string) *Tarefa {
    s.mu.Lock()
    defer s.mu.Unlock()

    t := &Tarefa{
        ID:        s.nextID,
        Titulo:    titulo,
        CriadaEm: time.Now(),
    }
    s.tarefas[s.nextID] = t
    s.nextID++
    return t
}

func (s *TarefaStore) Listar() []*Tarefa {
    s.mu.RLock()
    defer s.mu.RUnlock()

    lista := make([]*Tarefa, 0, len(s.tarefas))
    for _, t := range s.tarefas {
        lista = append(lista, t)
    }
    return lista
}

func (s *TarefaStore) Buscar(id int) (*Tarefa, bool) {
    s.mu.RLock()
    defer s.mu.RUnlock()
    t, ok := s.tarefas[id]
    return t, ok
}

func (s *TarefaStore) Deletar(id int) bool {
    s.mu.Lock()
    defer s.mu.Unlock()
    _, ok := s.tarefas[id]
    if ok {
        delete(s.tarefas, id)
    }
    return ok
}

// Handler
type TarefaHandler struct {
    store *TarefaStore
}

func (h *TarefaHandler) responderJSON(w http.ResponseWriter, status int, dados interface{}) {
    w.Header().Set("Content-Type", "application/json")
    w.WriteHeader(status)
    json.NewEncoder(w).Encode(dados)
}

func (h *TarefaHandler) responderErro(w http.ResponseWriter, status int, mensagem string) {
    h.responderJSON(w, status, map[string]string{"erro": mensagem})
}

// GET /tarefas — lista todas
// POST /tarefas — cria nova
func (h *TarefaHandler) handleTarefas(w http.ResponseWriter, r *http.Request) {
    switch r.Method {
    case http.MethodGet:
        h.responderJSON(w, http.StatusOK, h.store.Listar())

    case http.MethodPost:
        var req struct {
            Titulo string `json:"titulo"`
        }
        if err := json.NewDecoder(r.Body).Decode(&req); err != nil {
            h.responderErro(w, http.StatusBadRequest, "JSON inválido")
            return
        }
        if strings.TrimSpace(req.Titulo) == "" {
            h.responderErro(w, http.StatusBadRequest, "título é obrigatório")
            return
        }
        tarefa := h.store.Criar(req.Titulo)
        h.responderJSON(w, http.StatusCreated, tarefa)

    default:
        h.responderErro(w, http.StatusMethodNotAllowed, "método não permitido")
    }
}

// GET /tarefas/{id} — busca por ID
// DELETE /tarefas/{id} — deleta por ID
func (h *TarefaHandler) handleTarefaID(w http.ResponseWriter, r *http.Request) {
    // Extrai ID da URL
    partes := strings.Split(r.URL.Path, "/")
    id, err := strconv.Atoi(partes[len(partes)-1])
    if err != nil {
        h.responderErro(w, http.StatusBadRequest, "ID inválido")
        return
    }

    switch r.Method {
    case http.MethodGet:
        tarefa, ok := h.store.Buscar(id)
        if !ok {
            h.responderErro(w, http.StatusNotFound, "tarefa não encontrada")
            return
        }
        h.responderJSON(w, http.StatusOK, tarefa)

    case http.MethodDelete:
        if ok := h.store.Deletar(id); !ok {
            h.responderErro(w, http.StatusNotFound, "tarefa não encontrada")
            return
        }
        w.WriteHeader(http.StatusNoContent)

    default:
        h.responderErro(w, http.StatusMethodNotAllowed, "método não permitido")
    }
}

func main() {
    store := NewTarefaStore()
    // Dados iniciais
    store.Criar("Aprender Go")
    store.Criar("Construir uma API REST")
    store.Criar("Escrever testes")

    handler := &TarefaHandler{store: store}

    mux := http.NewServeMux()
    mux.HandleFunc("/tarefas", handler.handleTarefas)
    mux.HandleFunc("/tarefas/", handler.handleTarefaID)

    fmt.Println("API REST rodando em http://localhost:8080")
    fmt.Println("Endpoints:")
    fmt.Println("  GET    /tarefas        — lista todas")
    fmt.Println("  POST   /tarefas        — cria nova")
    fmt.Println("  GET    /tarefas/{id}   — busca por ID")
    fmt.Println("  DELETE /tarefas/{id}   — deleta por ID")

    log.Fatal(http.ListenAndServe(":8080", mux))
}
```

## 24.3 Cliente HTTP

```go
package main

import (
    "encoding/json"
    "fmt"
    "io"
    "net/http"
    "time"
)

type Post struct {
    UserID int    `json:"userId"`
    ID     int    `json:"id"`
    Titulo string `json:"title"`
    Corpo  string `json:"body"`
}

func main() {
    // Cliente HTTP com configurações
    client := &http.Client{
        Timeout: 10 * time.Second,
    }

    // GET simples
    resp, err := client.Get("https://jsonplaceholder.typicode.com/posts/1")
    if err != nil {
        fmt.Println("Erro:", err)
        return
    }
    defer resp.Body.Close()

    fmt.Println("Status:", resp.Status)
    fmt.Println("Content-Type:", resp.Header.Get("Content-Type"))

    // Ler e decodificar o corpo
    var post Post
    if err := json.NewDecoder(resp.Body).Decode(&post); err != nil {
        fmt.Println("Erro ao decodificar:", err)
        return
    }
    fmt.Printf("Post: ID=%d, Titulo=%s\n", post.ID, post.Titulo)

    // Ler corpo como string
    resp2, _ := client.Get("https://jsonplaceholder.typicode.com/posts/2")
    defer resp2.Body.Close()
    corpo, _ := io.ReadAll(resp2.Body)
    fmt.Println("Corpo como string:", string(corpo[:100])+"...")
}
```

---

# 25. CLI em Go

## 25.1 Argumentos de Linha de Comando

```go
package main

import (
    "flag"
    "fmt"
    "os"
    "strings"
)

func main() {
    // Lendo argumentos brutos
    fmt.Println("Programa:", os.Args[0])
    fmt.Println("Argumentos:", os.Args[1:])

    // Usando o pacote flag para argumentos nomeados
    nome := flag.String("nome", "Mundo", "Nome para saudar")
    vezes := flag.Int("vezes", 1, "Quantas vezes saudar")
    maiusculo := flag.Bool("maiusculo", false, "Usar maiúsculo")

    flag.Parse()

    saudacao := fmt.Sprintf("Olá, %s!", *nome)
    if *maiusculo {
        saudacao = strings.ToUpper(saudacao)
    }

    for i := 0; i < *vezes; i++ {
        fmt.Println(saudacao)
    }

    // Argumentos restantes após as flags
    args := flag.Args()
    if len(args) > 0 {
        fmt.Println("Argumentos adicionais:", args)
    }
}
```

Uso:

```bash
go run main.go -nome Alice -vezes 3 -maiusculo
go run main.go --help
```

## 25.2 Ferramenta CLI Completa

```go
package main

import (
    "bufio"
    "flag"
    "fmt"
    "os"
    "strings"
)

// Subcomandos
func cmdContar(args []string) {
    fs := flag.NewFlagSet("contar", flag.ExitOnError)
    linhas := fs.Bool("linhas", false, "contar linhas")
    palavras := fs.Bool("palavras", false, "contar palavras")
    fs.Parse(args)

    arquivo := fs.Arg(0)
    if arquivo == "" {
        fmt.Fprintln(os.Stderr, "Uso: cli contar [-linhas] [-palavras] <arquivo>")
        os.Exit(1)
    }

    f, err := os.Open(arquivo)
    if err != nil {
        fmt.Fprintf(os.Stderr, "Erro ao abrir arquivo: %v\n", err)
        os.Exit(1)
    }
    defer f.Close()

    contLinhas, contPalavras := 0, 0
    scanner := bufio.NewScanner(f)
    for scanner.Scan() {
        contLinhas++
        contPalavras += len(strings.Fields(scanner.Text()))
    }

    if *linhas {
        fmt.Printf("Linhas: %d\n", contLinhas)
    }
    if *palavras {
        fmt.Printf("Palavras: %d\n", contPalavras)
    }
    if !*linhas && !*palavras {
        fmt.Printf("Linhas: %d, Palavras: %d\n", contLinhas, contPalavras)
    }
}

func cmdBuscar(args []string) {
    fs := flag.NewFlagSet("buscar", flag.ExitOnError)
    ignorarCase := fs.Bool("i", false, "ignorar maiúsculas/minúsculas")
    fs.Parse(args)

    if fs.NArg() < 2 {
        fmt.Fprintln(os.Stderr, "Uso: cli buscar [-i] <padrão> <arquivo>")
        os.Exit(1)
    }

    padrao := fs.Arg(0)
    arquivo := fs.Arg(1)

    f, err := os.Open(arquivo)
    if err != nil {
        fmt.Fprintf(os.Stderr, "Erro: %v\n", err)
        os.Exit(1)
    }
    defer f.Close()

    if *ignorarCase {
        padrao = strings.ToLower(padrao)
    }

    scanner := bufio.NewScanner(f)
    linha := 0
    for scanner.Scan() {
        linha++
        texto := scanner.Text()
        comparar := texto
        if *ignorarCase {
            comparar = strings.ToLower(texto)
        }
        if strings.Contains(comparar, padrao) {
            fmt.Printf("%d: %s\n", linha, texto)
        }
    }
}

func main() {
    if len(os.Args) < 2 {
        fmt.Println("Uso: cli <comando> [opções]")
        fmt.Println("\nComandos:")
        fmt.Println("  contar  — conta linhas e palavras")
        fmt.Println("  buscar  — busca padrão em arquivo")
        os.Exit(1)
    }

    switch os.Args[1] {
    case "contar":
        cmdContar(os.Args[2:])
    case "buscar":
        cmdBuscar(os.Args[2:])
    default:
        fmt.Fprintf(os.Stderr, "Comando desconhecido: %s\n", os.Args[1])
        os.Exit(1)
    }
}
```

---

# 26. Boas Práticas

## 26.1 Nomes e Convenções

```go
package main

// CONVENÇÕES DE NOMENCLATURA EM GO

// Packages: curtos, minúsculos, sem underscores
// CORRETO: strconv, bufio, httputil
// ERRADO: string_convert, HTTPUtil

// Variáveis e funções: camelCase
// CORRETO: nomeUsuario, calcularTotal, isAtivo
// ERRADO: nome_usuario, CalcularTotal (se privado)

// Exportados: PascalCase (primeira letra maiúscula)
// CORRETO: NomeCompleto, CalcularTotal, MaxConexoes

// Acrônimos: todas maiúsculas
// CORRETO: userID, httpHandler, APIKey
// ERRADO: UserId, HttpHandler, ApiKey

// Interfaces: geralmente terminam em -er
// CORRETO: Reader, Writer, Stringer, Handler, Formatter

// Constantes de erro: Err + PascalCase
// CORRETO: ErrNotFound, ErrPermissionDenied

// TAMANHO DE NOMES: proporcional ao escopo
// Loop pequeno: i, j, k
// Função: n, err, buf
// Pacote: usuarioAtual, conexaoDB

func exemplo() {
    // Curto em escopo pequeno
    for i := 0; i < 10; i++ {
        _ = i
    }

    // Descritivo em escopo maior
    arquivosParaProcessar := []string{"a.txt", "b.txt"}
    _ = arquivosParaProcessar
}
```

## 26.2 Tratamento de Erros Idiomático

```go
package main

import (
    "errors"
    "fmt"
)

// RUIM: ignorar erros com _
func ruim() {
    dados, _ := lerArquivo("arquivo.txt")
    _ = dados
}

// BOM: tratar erros explicitamente
func bom() error {
    dados, err := lerArquivo("arquivo.txt")
    if err != nil {
        return fmt.Errorf("bom: %w", err)
    }
    _ = dados
    return nil
}

// RUIM: retornar erros genéricos
func buscarUsuarioRuim(id int) (string, error) {
    if id <= 0 {
        return "", errors.New("erro")
    }
    return "Alice", nil
}

// BOM: erros descritivos com contexto
var ErrIDInvalido = errors.New("ID inválido")

func buscarUsuarioBom(id int) (string, error) {
    if id <= 0 {
        return "", fmt.Errorf("buscarUsuario: id=%d: %w", id, ErrIDInvalido)
    }
    return "Alice", nil
}

// PADRÃO: early return para evitar aninhamento excessivo
func processarDadosRuim(dados []byte) (string, error) {
    if dados != nil {
        if len(dados) > 0 {
            resultado := string(dados)
            if resultado != "" {
                return resultado, nil
            } else {
                return "", errors.New("resultado vazio")
            }
        } else {
            return "", errors.New("dados vazios")
        }
    } else {
        return "", errors.New("dados nil")
    }
}

// MELHOR: early return
func processarDadosBom(dados []byte) (string, error) {
    if dados == nil {
        return "", errors.New("dados nil")
    }
    if len(dados) == 0 {
        return "", errors.New("dados vazios")
    }
    resultado := string(dados)
    if resultado == "" {
        return "", errors.New("resultado vazio")
    }
    return resultado, nil
}

func lerArquivo(caminho string) ([]byte, error) {
    return nil, fmt.Errorf("arquivo não encontrado: %s", caminho)
}

func main() {
    _ = bom()
    ruim()
    _ = buscarUsuarioRuim
    _, _ = buscarUsuarioBom(1)
}
```

## 26.3 Interfaces Pequenas

```go
package main

import "fmt"

// PRINCÍPIO: interfaces pequenas são mais úteis
// A interface io.Reader tem apenas 1 método:
// type Reader interface { Read(p []byte) (n int, err error) }

// RUIM: interface grande e rígida
type RepositorioGrande interface {
    CriarUsuario(nome, email string) error
    BuscarUsuarioPorID(id int) (string, error)
    BuscarUsuarioPorEmail(email string) (string, error)
    AtualizarUsuario(id int, nome string) error
    DeletarUsuario(id int) error
    ListarTodosUsuarios() ([]string, error)
    ContarUsuarios() (int, error)
}

// BOM: interfaces pequenas e compostas
type CriadorUsuario interface {
    CriarUsuario(nome, email string) error
}

type BuscadorUsuario interface {
    BuscarPorID(id int) (string, error)
}

type DeletadorUsuario interface {
    Deletar(id int) error
}

// Composição quando necessário
type RepositorioCompleto interface {
    CriadorUsuario
    BuscadorUsuario
    DeletadorUsuario
}

// Funções aceitam a MENOR interface necessária
func criarNovoUsuario(c CriadorUsuario, nome, email string) error {
    return c.CriarUsuario(nome, email)
}

// Implementação dummy
type MemoryRepo struct{}
func (r *MemoryRepo) CriarUsuario(nome, email string) error { return nil }
func (r *MemoryRepo) BuscarPorID(id int) (string, error)   { return "Alice", nil }
func (r *MemoryRepo) Deletar(id int) error                 { return nil }

func main() {
    repo := &MemoryRepo{}
    criarNovoUsuario(repo, "Alice", "alice@email.com")
    fmt.Println("OK")
}
```

---

# 27. Performance em Go

## 27.1 Profiling

```go
package main

import (
    "fmt"
    "os"
    "runtime/pprof"
    "time"
)

func operacaoIntensiva() {
    // Simulando processamento
    soma := 0
    for i := 0; i < 100_000_000; i++ {
        soma += i
    }
    _ = soma
}

func main() {
    // CPU Profile
    f, err := os.Create("cpu.prof")
    if err != nil {
        fmt.Println("Erro:", err)
        return
    }
    defer f.Close()

    pprof.StartCPUProfile(f)
    defer pprof.StopCPUProfile()

    inicio := time.Now()
    operacaoIntensiva()
    fmt.Printf("Tempo: %v\n", time.Since(inicio))

    // Memory Profile
    memF, _ := os.Create("mem.prof")
    defer memF.Close()
    pprof.WriteHeapProfile(memF)
}
```

```bash
# Gerar e analisar profiles
go build -o app main.go
./app

# Analisar CPU profile
go tool pprof cpu.prof

# Analisar no navegador
go tool pprof -http=:8081 cpu.prof

# Benchmark com teste
go test -bench=. -benchmem ./...
go test -bench=. -cpuprofile=cpu.prof -memprofile=mem.prof ./...
```

## 27.2 Benchmarks

```go
package main

import (
    "fmt"
    "strings"
    "testing"
)

// Para executar: go test -bench=. -benchmem

// Construção de string — forma lenta
func concatenarString(n int) string {
    s := ""
    for i := 0; i < n; i++ {
        s += fmt.Sprintf("item%d ", i)
    }
    return s
}

// Construção de string — forma rápida
func usarBuilder(n int) string {
    var sb strings.Builder
    for i := 0; i < n; i++ {
        fmt.Fprintf(&sb, "item%d ", i)
    }
    return sb.String()
}

func BenchmarkConcatenar(b *testing.B) {
    for i := 0; i < b.N; i++ {
        concatenarString(1000)
    }
}

func BenchmarkBuilder(b *testing.B) {
    for i := 0; i < b.N; i++ {
        usarBuilder(1000)
    }
}

func main() {
    fmt.Println("Execute com: go test -bench=. -benchmem")
}
```

## 27.3 Garbage Collector

```go
package main

import (
    "fmt"
    "runtime"
)

func main() {
    // Informações do GC
    var stats runtime.MemStats
    runtime.ReadMemStats(&stats)

    fmt.Printf("Alocado: %v bytes\n", stats.Alloc)
    fmt.Printf("Total alocado: %v bytes\n", stats.TotalAlloc)
    fmt.Printf("Uso do sistema: %v bytes\n", stats.Sys)
    fmt.Printf("Pausas GC: %v\n", stats.NumGC)

    // Dicas para reduzir pressão no GC:
    // 1. Reutilize objetos com sync.Pool
    // 2. Pre-aloque slices com capacidade adequada
    // 3. Evite alocações desnecessárias em hot paths

    // sync.Pool: reutilização de objetos
    // pool := sync.Pool{
    //     New: func() interface{} {
    //         return make([]byte, 1024)
    //     },
    // }
    // buf := pool.Get().([]byte)
    // defer pool.Put(buf)

    // Variável de ambiente para tunning do GC:
    // GOGC=100 (padrão): GC quando heap dobra
    // GOGC=off: desabilita GC
    // GOMEMLIMIT=100MiB: limite de memória (Go 1.19+)

    fmt.Println("NumCPU:", runtime.NumCPU())
    fmt.Println("NumGoroutine:", runtime.NumGoroutine())
    fmt.Println("GOMAXPROCS:", runtime.GOMAXPROCS(0))
}
```

---

# 28. Estrutura de Projetos Profissionais

## 28.1 Layout Padrão

```
meu-servico/
├── cmd/                    # Pontos de entrada (main packages)
│   ├── servidor/
│   │   └── main.go
│   └── cli/
│       └── main.go
├── internal/               # Código privado (não importável por outros módulos)
│   ├── api/
│   │   ├── handlers.go
│   │   ├── middleware.go
│   │   └── routes.go
│   ├── service/
│   │   ├── usuario.go
│   │   └── produto.go
│   ├── repository/
│   │   ├── usuario.go
│   │   └── produto.go
│   └── model/
│       ├── usuario.go
│       └── produto.go
├── pkg/                    # Código público (bibliotecas reutilizáveis)
│   ├── logger/
│   │   └── logger.go
│   └── validator/
│       └── validator.go
├── configs/                # Arquivos de configuração
│   ├── config.go
│   └── config.yaml
├── migrations/             # Migrações de banco de dados
│   ├── 001_create_users.sql
│   └── 002_create_products.sql
├── docs/                   # Documentação
├── scripts/                # Scripts de build/deploy
├── tests/                  # Testes de integração e e2e
├── go.mod
├── go.sum
├── Makefile
├── Dockerfile
└── README.md
```

## 28.2 Exemplo de Arquitetura Limpa

```go
// internal/model/usuario.go
package model

import "time"

type Usuario struct {
    ID         int       `json:"id" db:"id"`
    Nome       string    `json:"nome" db:"nome"`
    Email      string    `json:"email" db:"email"`
    SenhHash   string    `json:"-" db:"senha_hash"`
    CriadoEm  time.Time `json:"criado_em" db:"criado_em"`
}
```

```go
// internal/repository/usuario.go
package repository

import (
    "context"
    "meu-servico/internal/model"
)

// Interface define o contrato
type UsuarioRepository interface {
    Criar(ctx context.Context, u *model.Usuario) error
    BuscarPorID(ctx context.Context, id int) (*model.Usuario, error)
    BuscarPorEmail(ctx context.Context, email string) (*model.Usuario, error)
    Listar(ctx context.Context) ([]*model.Usuario, error)
    Deletar(ctx context.Context, id int) error
}

// Implementação em memória (para testes)
type MemoryUsuarioRepository struct {
    dados  map[int]*model.Usuario
    nextID int
}

func NewMemoryUsuarioRepository() *MemoryUsuarioRepository {
    return &MemoryUsuarioRepository{
        dados:  make(map[int]*model.Usuario),
        nextID: 1,
    }
}

// ... implementar todos os métodos da interface
```

```go
// internal/service/usuario.go
package service

import (
    "context"
    "errors"
    "fmt"
    "meu-servico/internal/model"
    "meu-servico/internal/repository"
)

var ErrEmailJaExiste = errors.New("email já cadastrado")
var ErrUsuarioNaoEncontrado = errors.New("usuário não encontrado")

type UsuarioService struct {
    repo repository.UsuarioRepository
}

func NewUsuarioService(repo repository.UsuarioRepository) *UsuarioService {
    return &UsuarioService{repo: repo}
}

func (s *UsuarioService) Registrar(ctx context.Context, nome, email, senha string) (*model.Usuario, error) {
    // Verificar se email já existe
    existente, _ := s.repo.BuscarPorEmail(ctx, email)
    if existente != nil {
        return nil, ErrEmailJaExiste
    }

    // Criar usuário (em produção, hashearia a senha)
    usuario := &model.Usuario{
        Nome:  nome,
        Email: email,
    }

    if err := s.repo.Criar(ctx, usuario); err != nil {
        return nil, fmt.Errorf("registrar usuário: %w", err)
    }

    return usuario, nil
}
```

---

# 29. Projeto Final — API REST Completa

Vamos criar uma API REST completa para gerenciamento de tarefas com:

- CRUD completo
- Autenticação JWT simples
- Middleware de logging e CORS
- Tratamento de erros padronizado

```go
// main.go — ponto de entrada
package main

import (
    "context"
    "fmt"
    "log"
    "net/http"
    "os"
    "os/signal"
    "syscall"
    "time"
)

func main() {
    servidor := NovoServidor()

    // Servidor HTTP com graceful shutdown
    httpServer := &http.Server{
        Addr:         ":8080",
        Handler:      servidor.mux,
        ReadTimeout:  15 * time.Second,
        WriteTimeout: 15 * time.Second,
        IdleTimeout:  60 * time.Second,
    }

    // Canal para sinais do SO
    quit := make(chan os.Signal, 1)
    signal.Notify(quit, syscall.SIGINT, syscall.SIGTERM)

    // Iniciar servidor em goroutine
    go func() {
        fmt.Printf("Servidor rodando em http://localhost%s\n", httpServer.Addr)
        if err := httpServer.ListenAndServe(); err != nil && err != http.ErrServerClosed {
            log.Fatalf("Erro no servidor: %v", err)
        }
    }()

    // Aguardar sinal de encerramento
    <-quit
    fmt.Println("\nEncerrando servidor graciosamente...")

    ctx, cancel := context.WithTimeout(context.Background(), 30*time.Second)
    defer cancel()

    if err := httpServer.Shutdown(ctx); err != nil {
        log.Printf("Erro no shutdown: %v", err)
    }

    fmt.Println("Servidor encerrado.")
}
```

```go
// servidor.go
package main

import (
    "encoding/json"
    "fmt"
    "log"
    "net/http"
    "strconv"
    "strings"
    "sync"
    "time"
)

// ============ MODELOS ============

type Tarefa struct {
    ID         int       `json:"id"`
    UserID     int       `json:"user_id"`
    Titulo     string    `json:"titulo"`
    Descricao  string    `json:"descricao,omitempty"`
    Feita      bool      `json:"feita"`
    Prioridade string    `json:"prioridade"` // alta, media, baixa
    Tags       []string  `json:"tags,omitempty"`
    CriadaEm  time.Time `json:"criada_em"`
    AtualizadaEm time.Time `json:"atualizada_em"`
}

type RespostaErro struct {
    Erro    string `json:"erro"`
    Detalhe string `json:"detalhe,omitempty"`
}

type RespostaPaginada struct {
    Dados  interface{} `json:"dados"`
    Total  int         `json:"total"`
    Pagina int         `json:"pagina"`
}

// ============ REPOSITÓRIO ============

type TarefaRepo struct {
    mu      sync.RWMutex
    tarefas map[int]*Tarefa
    nextID  int
}

func NewTarefaRepo() *TarefaRepo {
    repo := &TarefaRepo{
        tarefas: make(map[int]*Tarefa),
        nextID:  1,
    }
    // Dados de exemplo
    repo.Criar(1, "Estudar Go", "Completar o mega tutorial", "alta", []string{"golang", "programação"})
    repo.Criar(1, "Escrever testes", "Cobertura de 80%+", "media", []string{"testes", "qualidade"})
    repo.Criar(2, "Revisar PRs", "3 PRs pendentes", "alta", nil)
    return repo
}

func (r *TarefaRepo) Criar(userID int, titulo, desc, prioridade string, tags []string) *Tarefa {
    r.mu.Lock()
    defer r.mu.Unlock()

    agora := time.Now()
    t := &Tarefa{
        ID:           r.nextID,
        UserID:       userID,
        Titulo:       titulo,
        Descricao:    desc,
        Prioridade:   prioridade,
        Tags:         tags,
        CriadaEm:    agora,
        AtualizadaEm: agora,
    }
    r.tarefas[r.nextID] = t
    r.nextID++
    return t
}

func (r *TarefaRepo) ListarPorUser(userID int) []*Tarefa {
    r.mu.RLock()
    defer r.mu.RUnlock()

    var lista []*Tarefa
    for _, t := range r.tarefas {
        if t.UserID == userID {
            lista = append(lista, t)
        }
    }
    return lista
}

func (r *TarefaRepo) BuscarPorID(id, userID int) (*Tarefa, bool) {
    r.mu.RLock()
    defer r.mu.RUnlock()
    t, ok := r.tarefas[id]
    if !ok || t.UserID != userID {
        return nil, false
    }
    return t, true
}

func (r *TarefaRepo) Atualizar(id, userID int, titulo, desc string, feita bool, prioridade string) (*Tarefa, bool) {
    r.mu.Lock()
    defer r.mu.Unlock()
    t, ok := r.tarefas[id]
    if !ok || t.UserID != userID {
        return nil, false
    }
    t.Titulo = titulo
    t.Descricao = desc
    t.Feita = feita
    t.Prioridade = prioridade
    t.AtualizadaEm = time.Now()
    return t, true
}

func (r *TarefaRepo) Deletar(id, userID int) bool {
    r.mu.Lock()
    defer r.mu.Unlock()
    t, ok := r.tarefas[id]
    if !ok || t.UserID != userID {
        return false
    }
    delete(r.tarefas, id)
    return true
}

// ============ SERVIDOR ============

type Servidor struct {
    mux  *http.ServeMux
    repo *TarefaRepo
}

func NovoServidor() *Servidor {
    s := &Servidor{
        mux:  http.NewServeMux(),
        repo: NewTarefaRepo(),
    }
    s.configurarRotas()
    return s
}

func (s *Servidor) configurarRotas() {
    // Aplicar middlewares
    handler := func(path string, h http.HandlerFunc) {
        s.mux.Handle(path, s.middlewareLog(s.middlewareCORS(s.middlewareAuth(h))))
    }

    // Rotas públicas (sem auth)
    s.mux.Handle("/health", s.middlewareLog(http.HandlerFunc(s.handleHealth)))

    // Rotas autenticadas
    handler("/tarefas", s.handleTarefas)
    handler("/tarefas/", s.handleTarefaID)
}

// ============ MIDDLEWARE ============

func (s *Servidor) middlewareLog(next http.Handler) http.Handler {
    return http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
        inicio := time.Now()
        rw := &responseWriter{ResponseWriter: w, status: 200}
        next.ServeHTTP(rw, r)
        log.Printf("[%s] %s %s %d %v",
            r.Method, r.URL.Path, r.RemoteAddr, rw.status, time.Since(inicio))
    })
}

type responseWriter struct {
    http.ResponseWriter
    status int
}

func (rw *responseWriter) WriteHeader(status int) {
    rw.status = status
    rw.ResponseWriter.WriteHeader(status)
}

func (s *Servidor) middlewareCORS(next http.Handler) http.Handler {
    return http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
        w.Header().Set("Access-Control-Allow-Origin", "*")
        w.Header().Set("Access-Control-Allow-Methods", "GET, POST, PUT, DELETE, OPTIONS")
        w.Header().Set("Access-Control-Allow-Headers", "Content-Type, Authorization")

        if r.Method == http.MethodOptions {
            w.WriteHeader(http.StatusNoContent)
            return
        }
        next.ServeHTTP(w, r)
    })
}

// Auth simplificado — em produção, use JWT real
func (s *Servidor) middlewareAuth(next http.Handler) http.Handler {
    return http.HandlerFunc(func(w http.ResponseWriter, r *http.Request) {
        token := r.Header.Get("Authorization")
        token = strings.TrimPrefix(token, "Bearer ")

        userID := 0
        switch token {
        case "token-alice":
            userID = 1
        case "token-bob":
            userID = 2
        default:
            s.responderErro(w, http.StatusUnauthorized, "token inválido", "")
            return
        }

        // Adicionar userID ao contexto seria o ideal
        // Por simplicidade, usaremos query param como fallback
        r.Header.Set("X-User-ID", strconv.Itoa(userID))
        next.ServeHTTP(w, r)
    })
}

// ============ HELPERS ============

func (s *Servidor) responderJSON(w http.ResponseWriter, status int, dados interface{}) {
    w.Header().Set("Content-Type", "application/json; charset=utf-8")
    w.WriteHeader(status)
    if err := json.NewEncoder(w).Encode(dados); err != nil {
        log.Printf("Erro ao serializar resposta: %v", err)
    }
}

func (s *Servidor) responderErro(w http.ResponseWriter, status int, erro, detalhe string) {
    s.responderJSON(w, status, RespostaErro{Erro: erro, Detalhe: detalhe})
}

func (s *Servidor) getUserID(r *http.Request) int {
    id, _ := strconv.Atoi(r.Header.Get("X-User-ID"))
    return id
}

// ============ HANDLERS ============

func (s *Servidor) handleHealth(w http.ResponseWriter, r *http.Request) {
    s.responderJSON(w, http.StatusOK, map[string]string{
        "status": "ok",
        "hora":   time.Now().Format(time.RFC3339),
    })
}

func (s *Servidor) handleTarefas(w http.ResponseWriter, r *http.Request) {
    userID := s.getUserID(r)

    switch r.Method {
    case http.MethodGet:
        tarefas := s.repo.ListarPorUser(userID)
        if tarefas == nil {
            tarefas = []*Tarefa{}
        }
        s.responderJSON(w, http.StatusOK, RespostaPaginada{
            Dados:  tarefas,
            Total:  len(tarefas),
            Pagina: 1,
        })

    case http.MethodPost:
        var req struct {
            Titulo     string   `json:"titulo"`
            Descricao  string   `json:"descricao"`
            Prioridade string   `json:"prioridade"`
            Tags       []string `json:"tags"`
        }
        if err := json.NewDecoder(r.Body).Decode(&req); err != nil {
            s.responderErro(w, http.StatusBadRequest, "JSON inválido", err.Error())
            return
        }
        if strings.TrimSpace(req.Titulo) == "" {
            s.responderErro(w, http.StatusBadRequest, "título é obrigatório", "")
            return
        }
        if req.Prioridade == "" {
            req.Prioridade = "media"
        }
        validas := map[string]bool{"alta": true, "media": true, "baixa": true}
        if !validas[req.Prioridade] {
            s.responderErro(w, http.StatusBadRequest, "prioridade inválida", "use: alta, media ou baixa")
            return
        }
        tarefa := s.repo.Criar(userID, req.Titulo, req.Descricao, req.Prioridade, req.Tags)
        s.responderJSON(w, http.StatusCreated, tarefa)

    default:
        s.responderErro(w, http.StatusMethodNotAllowed, "método não permitido", "")
    }
}

func (s *Servidor) handleTarefaID(w http.ResponseWriter, r *http.Request) {
    userID := s.getUserID(r)

    partes := strings.Split(strings.TrimPrefix(r.URL.Path, "/tarefas/"), "/")
    id, err := strconv.Atoi(partes[0])
    if err != nil || id <= 0 {
        s.responderErro(w, http.StatusBadRequest, "ID inválido", "")
        return
    }

    switch r.Method {
    case http.MethodGet:
        tarefa, ok := s.repo.BuscarPorID(id, userID)
        if !ok {
            s.responderErro(w, http.StatusNotFound, "tarefa não encontrada", "")
            return
        }
        s.responderJSON(w, http.StatusOK, tarefa)

    case http.MethodPut:
        var req struct {
            Titulo     string `json:"titulo"`
            Descricao  string `json:"descricao"`
            Feita      bool   `json:"feita"`
            Prioridade string `json:"prioridade"`
        }
        if err := json.NewDecoder(r.Body).Decode(&req); err != nil {
            s.responderErro(w, http.StatusBadRequest, "JSON inválido", err.Error())
            return
        }
        tarefa, ok := s.repo.Atualizar(id, userID, req.Titulo, req.Descricao, req.Feita, req.Prioridade)
        if !ok {
            s.responderErro(w, http.StatusNotFound, "tarefa não encontrada", "")
            return
        }
        s.responderJSON(w, http.StatusOK, tarefa)

    case http.MethodDelete:
        if ok := s.repo.Deletar(id, userID); !ok {
            s.responderErro(w, http.StatusNotFound, "tarefa não encontrada", "")
            return
        }
        w.WriteHeader(http.StatusNoContent)

    default:
        s.responderErro(w, http.StatusMethodNotAllowed, "método não permitido", "")
    }
}

// Função auxiliar para o servidor standalone
func init() {
    fmt.Println("Inicializando servidor de tarefas...")
}
```

### Testando a API

```bash
# Health check
curl http://localhost:8080/health

# Listar tarefas da Alice
curl -H "Authorization: Bearer token-alice" http://localhost:8080/tarefas

# Criar tarefa
curl -X POST \
  -H "Authorization: Bearer token-alice" \
  -H "Content-Type: application/json" \
  -d '{"titulo":"Nova tarefa","descricao":"Descrição","prioridade":"alta","tags":["urgente"]}' \
  http://localhost:8080/tarefas

# Buscar tarefa
curl -H "Authorization: Bearer token-alice" http://localhost:8080/tarefas/1

# Atualizar tarefa
curl -X PUT \
  -H "Authorization: Bearer token-alice" \
  -H "Content-Type: application/json" \
  -d '{"titulo":"Tarefa atualizada","feita":true,"prioridade":"baixa"}' \
  http://localhost:8080/tarefas/1

# Deletar tarefa
curl -X DELETE \
  -H "Authorization: Bearer token-alice" \
  http://localhost:8080/tarefas/1
```

---

# 30. Conclusão

## 30.1 O Que Você Aprendeu

Ao longo deste tutorial, cobrimos Go do zero ao avançado:

**Fundamentos:**

- Instalação e configuração do ambiente Go
- Estrutura de programas Go, packages e o runtime
- Tipos primitivos: int, float, string, bool, byte, rune
- Operadores aritméticos, lógicos e bitwise
- Controle de fluxo: if/else, switch, for (o único loop)

**Estruturas de Dados:**

- Arrays (tamanho fixo, passagem por valor)
- Slices (dinâmicos, fundamentais em Go, entendemos o header interno)
- Maps (tabelas hash, verificação de existência com comma-ok)

**Tipos Compostos e OOP em Go:**

- Structs com campos e struct tags
- Métodos com value e pointer receivers
- Interfaces com implementação implícita
- Composição via embedding (no place de herança)
- Ponteiros e quando usá-los

**Organização de Código:**

- Pacotes e exportação de identificadores
- Sistema de módulos com go.mod
- Estrutura de projetos profissionais (Clean Architecture)

**I/O e Rede:**

- Leitura e escrita de arquivos
- Tratamento robusto de erros com wrapping
- JSON marshal/unmarshal
- Servidor HTTP e clientes HTTP

**Concorrência:**

- Goroutines (threads leves do Go)
- Channels (comunicação entre goroutines)
- select para multiplexação de channels
- Worker pools e pipelines
- Mutex, WaitGroup, Once e sync.Map

**Avançado:**

- Context para cancelamento e timeout
- Profiling e benchmarking
- Graceful shutdown de servidores
- CLI com subcomandos e flags

## 30.2 Próximos Passos

Agora que você domina os fundamentos, aqui está um caminho sugerido:

### Frameworks e Bibliotecas Essenciais

```
Frameworks Web:
├── Gin — roteamento eficiente, amplamente usado
├── Echo — similar ao Gin, API mais limpa
├── Chi — leve, baseado na stdlib
└── Fiber — inspirado no Express.js, muito performático

ORMs e Banco de Dados:
├── GORM — ORM popular, suporta PostgreSQL, MySQL, SQLite
├── sqlx — extensão do database/sql com mais comodidades
└── pgx — driver nativo PostgreSQL, máxima performance

Logging:
├── zap (Uber) — extremamente performático
└── slog — biblioteca padrão desde Go 1.21

Configuração:
├── viper — configuração multi-fonte
└── envconfig — configuração via variáveis de ambiente

Testes:
├── testify — asserções e mocks
└── gomock — geração de mocks

Utilitários:
├── validator — validação de structs
└── cobra — criação de CLIs complexas
```

### Conceitos para Aprofundar

- **Generics** (Go 1.18+): tipos paramétricos para reutilização de código
- **Reflection**: `reflect` package para programação dinâmica
- **cgo**: integração com código C
- **WebAssembly**: compilar Go para wasm
- **gRPC**: comunicação entre microsserviços com Protocol Buffers
- **Testes avançados**: tabela de testes, subtestes, mocks, testes de integração

## 30.3 Recursos Oficiais

- **Documentação oficial**: https://go.dev/doc/
- **Tour of Go (interativo)**: https://go.dev/tour/
- **Go Playground**: https://go.dev/play/
- **Effective Go**: https://go.dev/doc/effective_go
- **Especificação da linguagem**: https://go.dev/ref/spec
- **Go Blog**: https://go.dev/blog/
- **pkg.go.dev**: documentação de pacotes

## 30.4 Filosofia Final

Go é uma linguagem que recompensa a simplicidade. Não tente trazer padrões de outras linguagens para o Go — abrace as idiomias do Go:

- Erros são valores, não exceções
- Composição sobre herança
- Interfaces implícitas promovem desacoplamento
- Concorrência com channels é mais segura que mutexes em muitos casos
- Código legível é mais valioso que código "inteligente"
- `gofmt` resolve todos os debates de formatação

Como disse Rob Pike:

> _"Clarity is indeed the most important quality of Go code."_

---


