---
title: Usar os modelos de Aplicativo de Página Única com o ASP.NET Core
author: SteveSandersonMS
description: Saiba como instalar e começar a trabalhar com os modelos de projeto do SPA (Aplicativo de Página Única) ASP.NET Core.
monikerRange: '>= aspnetcore-2.0'
ms.author: scaddie
ms.custom: mvc
ms.date: 02/21/2018
uid: spa/index
ms.openlocfilehash: ab164ae5d2df47739ec04b32cd21835ffdf9f87f
ms.sourcegitcommit: a1afd04758e663d7062a5bfa8a0d4dca38f42afc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/20/2018
ms.locfileid: "36291439"
---
# <a name="use-the-single-page-application-templates-with-aspnet-core"></a>Usar os modelos de Aplicativo de Página Única com o ASP.NET Core

::: moniker range="= aspnetcore-2.0"

> [!NOTE]
> O SDK do .NET Core 2.0.x inclui modelos de projeto mais antigos para Angular, React e React with Redux. Esta documentação não é sobre esses modelos de projeto antigos. Essa documentação é para os modelos Angular, React e React with Redux mais recentes, que podem ser instalados manualmente no ASP.NET Core 2.0. Os modelos são incluídos por padrão com o ASP.NET Core 2.1.

::: moniker-end

## <a name="prerequisites"></a>Pré-requisitos

* [!INCLUDE [](~/includes/net-core-sdk-download-link.md)]
* [Node.js](https://nodejs.org), versão 6 ou posterior

## <a name="installation"></a>Instalação

::: moniker range=">= aspnetcore-2.1"

Os modelos já estão instalados com o ASP.NET Core 2.1.

::: moniker-end

::: moniker range="= aspnetcore-2.0"

Se você tiver o ASP.NET Core 2.0, execute o seguinte comando para instalar os modelos do ASP.NET Core atualizados para Angular, React e React with Redux:

```console
dotnet new --install Microsoft.DotNet.Web.Spa.ProjectTemplates::2.0.0
```

::: moniker-end

## <a name="use-the-templates"></a>Usar os modelos

* [Usar o modelo de projeto Angular](xref:spa/angular)
* [Usar o modelo de projeto React](xref:spa/react)
* [Usar o modelo de projeto React with Redux](xref:spa/react-with-redux)
