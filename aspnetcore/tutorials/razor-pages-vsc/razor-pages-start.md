---
title: Introdução a Páginas Razor do ASP.NET Core no Visual Studio Code
author: rick-anderson
description: Conheça as noções básicas da criação de um aplicativo Web Páginas Razor do ASP.NET Core Razor com o Visual Studio Code.
monikerRange: '>= aspnetcore-2.0'
ms.author: riande
ms.date: 08/27/2017
uid: tutorials/razor-pages-vsc/razor-pages-start
ms.openlocfilehash: b1f1dcc1401d707cff79f3269ab70b900e9fc21c
ms.sourcegitcommit: b8a2f14bf8dd346d7592977642b610bbcb0b0757
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2018
ms.locfileid: "38123377"
---
# <a name="get-started-with-aspnet-core-razor-pages-in-visual-studio-code"></a>Introdução a Páginas Razor do ASP.NET Core no Visual Studio Code

Por [Rick Anderson](https://twitter.com/RickAndMSFT)

Este tutorial ensina as noções básicas de criação de um aplicativo Web de Páginas do Razor do ASP.NET Core. Recomendamos que você conclua a [Introdução a Páginas do Razor](xref:razor-pages/index) antes de iniciar este tutorial. Páginas do Razor é a maneira recomendada para criar a interface do usuário para aplicativos Web no ASP.NET Core.

## <a name="prerequisites"></a>Pré-requisitos

[!INCLUDE [](~/includes/net-core-prereqs-vscode.md)]

## <a name="create-a-razor-web-app"></a>Criar um aplicativo Web do Razor

Em um terminal, execute os seguintes comandos:

::: moniker range=">= aspnetcore-2.1"

```console
dotnet new webapp -o RazorPagesMovie
cd RazorPagesMovie
dotnet run
```

[!INCLUDE[](~/includes/webapp-alias-notice.md)]

::: moniker-end

::: moniker range="= aspnetcore-2.0"

```console
dotnet new razor -o RazorPagesMovie
cd RazorPagesMovie
dotnet run
```

::: moniker-end

Os comandos anteriores usam a [CLI do .NET Core](https://docs.microsoft.com/dotnet/core/tools/dotnet) para criar e executar um projeto de Páginas do Razor. Abra um navegador em http://localhost:5000 para exibir o aplicativo.

![Página Inicial ou de Índice](../razor-pages/razor-pages-start/_static/home.png)

[!INCLUDE [razor-pages-start](../../includes/RP/razor-pages-start.md)]

## <a name="open-the-project"></a>Abrir o projeto

Pressione Ctrl + C para encerrar o aplicativo.

No Visual Studio Code (VSCode), selecione **Arquivo > Abrir Pasta** e, em seguida, selecione a pasta *RazorPagesMovie*.

- Selecione **Sim** para a mensagem de **Aviso** "Os ativos necessários para criar e depurar estão ausentes no 'RazorPagesMovie'. Deseja adicioná-los?"
- Selecione **Restaurar** para a mensagem **Informativa** "Há dependências não resolvidas".

### <a name="launch-the-app"></a>Iniciar o aplicativo

Pressione Ctrl+F5 para iniciar o aplicativo sem depuração. Alternativamente, do menu **Depurar**, selecione **Iniciar Sem Depurar**.

No próximo tutorial, adicionaremos um modelo para o projeto. 

> [!div class="step-by-step"]
> [Próximo: adicionando um modelo](xref:tutorials/razor-pages-vsc/model)  
