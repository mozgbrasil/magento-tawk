[checkmark]: https://raw.githubusercontent.com/mozgbrasil/mozgbrasil.github.io/master/assets/images/logos/logo_32_32.png "MOZG"
![valid XHTML][checkmark]

[psr4]: http://www.php-fig.org/psr/psr-4/
[getcomposer]: https://getcomposer.org/
[uninstall-mods]: https://getcomposer.org/doc/03-cli.md#remove

# Tawk/Widget

## Sinopse

Módulo para Magento

## Motivação

Automação para a instalação do módulo

Para mais informações, visite

https://www.tawk.to/knowledgebase/plugins-and-modules/magento-integration/

Note que não somos o desenvolvedor desta extensão

Esse repositório foi criado com o intuito de instalar o módulo via composer

Neste repositório foi adicionado somente o suporte ao composer e modman.

## Suporte / Dúvidas

Para obter o devido suporte entre em contato com a desenvolvedora do módulo

## Instalação - Atualização - Desinstalação - Desativação

Esta biblioteca destina-se a ser instalado usando o [Composer][getcomposer].

--

Certique se da presença do arquivo composer.json na raiz do seu projeto Magento e que o mesmo tenha os parâmetros semelhantes ao modelo JSON abaixo

	{
	  "minimum-stability": "dev",
	  "prefer-stable": true,
	  "license": [
	    "proprietary"
	  ],
	  "repositories": [
	    {
	      "type": "vcs",
	      "url":  "git@github.com:mozgbrasil/magento-tawk.git"
	    },
	    {
	      "type": "composer",
	      "url": "https://packages.firegento.com"
	    }
	  ],
	  "extra": {
	    "magento-root-dir": "./",
	    "magento-deploystrategy": "copy",
	    "magento-force": true
	  }
	}

Caso não exista o arquivo composer.json na raiz do projeto Magento, crie o mesmo adicionado o conteúdo acima

--

Antes de efetuar qualquer atualização no Magento sempre mantenha o Compiler e o Cache desativado

--

### Para instalar o módulo execute o comando a seguir no terminal do seu servidor

	composer require mozgbrasil/magento-tawk:dev-master

Você pode verificar se o módulo está instalado, indo ao backend em:

	STORES -> Configuration -> ADVANCED/Advanced -> Disable Modules Output

--

### Para atualizar o módulo execute o comando a seguir no terminal do seu servidor

	composer update

Na ocorrência de erro, renomeie a pasta /vendor/mozgbrasil e execute novamente

Para checar a data do módulo execute o seguinte comando

	grep -ri --include=*.json 'time": "' ./vendor/mozgbrasil

--

### Para [desinstalar][uninstall-mods] o módulo execute o comando a seguir no terminal do seu servidor

	composer remove mozgbrasil/magento-tawk

--

### Para desativar o módulo

1. Antes de efetuar qualquer processo que envolva atualização sobre o Magento é necessário manter o Compiler e Cache desativado

2. Caso queira desativar os módulos da MOZG renomeie a seguinte pasta app/code/community/Hibrido

A desativação do módulo pode ser usado para detectar se determinada ocorrência tem relação com o módulo

--

## Perguntas mais frequentes "FAQ"

### ?

## Badges

[![Join the chat at https://gitter.im/mozgbrasil](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/mozgbrasil/)
[![Latest Stable Version](https://poser.pugx.org/mozgbrasil/magento-tawk/v/stable)](https://packagist.org/packages/mozgbrasil/magento-tawk)
[![Total Downloads](https://poser.pugx.org/mozgbrasil/magento-tawk/downloads)](https://packagist.org/packages/mozgbrasil/magento-tawk)
[![Latest Unstable Version](https://poser.pugx.org/mozgbrasil/magento-tawk/v/unstable)](https://packagist.org/packages/mozgbrasil/magento-tawk)
[![License](https://poser.pugx.org/mozgbrasil/magento-tawk/license)](https://packagist.org/packages/mozgbrasil/magento-tawk)
[![Monthly Downloads](https://poser.pugx.org/mozgbrasil/magento-tawk/d/monthly)](https://packagist.org/packages/mozgbrasil/magento-tawk)
[![Daily Downloads](https://poser.pugx.org/mozgbrasil/magento-tawk/d/daily)](https://packagist.org/packages/mozgbrasil/magento-tawk)
[![Reference Status](https://www.versioneye.com/php/mozgbrasil:magento-tawk/reference_badge.svg?style=flat-square)](https://www.versioneye.com/php/mozgbrasil:magento-tawk/references)
[![Dependency Status](https://www.versioneye.com/php/mozgbrasil:magento-tawk/1.0.0/badge?style=flat-square)](https://www.versioneye.com/php/mozgbrasil:magento-tawk/1.0.0)

:cat2:
