# Utilizando a ferramenta de teste "JEST"

#### Exportando a função como um modulo para poder ser acessada no outro arquivo
- Esta linha de código deve ser escrita no arquivo onde se encontra a sua função
```js
module.exports = suaFunção;
```

#### Chamando a função no arquivo de teste
- Esta linha de código deve ser escrita no arquivo de teste
```js
const suaFunção = require("Caminho até o arquivo onde se encontra a função");
```

#### Função para executar o teste e retornar se deu certo ou não
- Esta linha de código deve ser escrita no arquivo de teste
```js 
test("Mensagem para exibir", () => {
    expect(suaFuncao(valor1, valor2)).toBe(resultado)
})
```

## Executar o teste, pelo prompt de comando
- Código no prompt de comando
```js
npm test
```

## Gerar um relatório de teste
- Código no prompt de comando
```js
npx jest  --coverage
```