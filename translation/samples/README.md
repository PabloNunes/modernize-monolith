# 📦 Amostras Iniciais do Workshop

Esta pasta contém as amostras iniciais (starter samples) para cada módulo prático do workshop.

## 📁 Estrutura

```
samples/
├── 02-upgrade-dotnet-start/          # Módulo 2: Atualização do .NET
├── 03-modernize-copilot-start/       # Módulo 3: Modernização com Copilot
└── 04-ai-capabilities-start/         # Módulo 4: Incorporando IA
```

## 🚀 Como Usar

### Módulo 2: Atualização do .NET

**Pasta**: `02-upgrade-dotnet-start/`

Esta amostra contém a aplicação eShopLite em .NET Framework 4.8 que será atualizada para .NET 9.

**Para começar:**
1. Navegue até a pasta: `cd 02-upgrade-dotnet-start`
2. Abra a solution no Visual Studio: `eShopLiteFx.sln`
3. Siga as instruções no [Módulo 2: Atualização do .NET](../02-atualizacao-dotnet.md)

**Estrutura:**
- `src/eShopLite.StoreFx/` - Projeto ASP.NET MVC em .NET Framework 4.8

### Módulo 3: Modernização com Copilot

**Pasta**: `03-modernize-copilot-start/`

Esta amostra contém a aplicação eShopLite já atualizada para .NET 9, mas ainda usando padrões legados que serão modernizados.

**Para começar:**
1. Navegue até a pasta: `cd 03-modernize-copilot-start`
2. Abra a solution no Visual Studio: `eShopLite.sln`
3. Siga as instruções no [Módulo 3: Modernização com Copilot](../03-modernizacao-copilot.md)

**Estrutura:**
- `src/eShopLite.StoreCore/` - Projeto .NET 9 a ser modernizado

### Módulo 4: Incorporando IA

**Pasta**: `04-ai-capabilities-start/`

Esta amostra contém a aplicação eShopLite modernizada com arquitetura de microserviços usando .NET Aspire, pronta para receber capacidades de IA.

**Para começar:**
1. Navegue até a pasta: `cd 04-ai-capabilities-start`
2. Abra a solution no Visual Studio: `eShopLite.sln`
3. Siga as instruções no [Módulo 4: Incorporando IA](../04-incorporando-ia.md)

**Estrutura:**
- `src/eShopLite.AppHost/` - Host do .NET Aspire
- `src/eShopLite.Store/` - Aplicação frontend Blazor
- `src/eShopLite.Products/` - API de produtos
- `src/eShopLite.StoreInfo/` - API de informações da loja
- `src/eShopLite.ServiceDefaults/` - Configurações compartilhadas

## 📋 Requisitos

Certifique-se de ter instalado:

- [Visual Studio 2022](https://visualstudio.microsoft.com/pt-br/vs/) ou superior
- [.NET 9 SDK](https://dotnet.microsoft.com/pt-br/download/dotnet/9.0)
- [.NET Framework 4.8](https://dotnet.microsoft.com/pt-br/download/dotnet-framework/net48) (para módulo 2)
- [GitHub Copilot](https://github.com/features/copilot) instalado no Visual Studio
- [SQL Server Express](https://www.microsoft.com/pt-br/download/details.aspx?id=104781) (opcional, para módulo 2)

## 💡 Dicas

- **Crie uma cópia**: Antes de começar cada módulo, considere fazer uma cópia da pasta da amostra para preservar o estado original
- **Use controle de versão**: Inicialize um repositório Git em cada projeto para rastrear suas mudanças:
  ```bash
  cd 02-upgrade-dotnet-start
  git init
  git add .
  git commit -m "Initial commit - starter sample"
  ```
- **Siga a ordem**: Os módulos são progressivos, então recomenda-se seguir na ordem apresentada

## 🔗 Recursos Adicionais

- [Documentação completa do workshop](../README.md)
- [Repositório original](https://github.com/PabloNunes/modernize-monolith)
- [Módulo 1: Configurando o Ambiente](../01-configurando-ambiente.md)

## ❓ Problemas Comuns

### Erro ao abrir a solution

Se você receber um erro ao abrir a solution, certifique-se de ter:
- Visual Studio 2022 atualizado
- Todas as cargas de trabalho necessárias instaladas (ASP.NET, .NET desktop development)

### Pacotes NuGet não restauram

Execute no terminal:
```bash
dotnet restore
```

### Build falha

Certifique-se de que:
1. Você tem o SDK correto instalado (verifique com `dotnet --version`)
2. Todas as dependências foram restauradas
3. Não há conflitos de versão

---

**Nota**: Estas amostras são cópias dos projetos originais do repositório principal. Para a versão mais atualizada, consulte o [repositório original](https://github.com/PabloNunes/modernize-monolith).
