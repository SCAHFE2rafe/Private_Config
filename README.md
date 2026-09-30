# Aviso


---

O material foi montado acompanhando um curso aberto. O conteúdo original não é meu e não deve ser redistribuído.

Se quiser estudar o assunto a fundo, procure o curso na plataforma de origem.


# Geral

A unidade trata de gerenciamento de dependências e ciclo de build da linguagem.

## Projetos com vários módulos

![estrutura de módulos](images/maven-multimodule-projects.png)

Gerei os módulos rodando o assistente interativo na raiz do projeto anterior. No assistente em si não precisei mexer em nada — a alteração vai no comando que ele produz.

A alternativa é passar o identificador do artefato direto na linha de comando, ou responder com o valor certo quando ele perguntar.

O que mudou no arquivo de configuração principal:

![módulos no pom](images/modules-in-pom-xml.png)

Além disso, os diretórios dos módulos apareceram no disco, ao lado do diretório principal:

![módulos no sistema de arquivos](images/modules-in-filesystem.png)

Outro detalhe: dentro de cada módulo gerado, o arquivo de configuração ganha uma seção apontando para o projeto pai. A imagem seguinte compara o arquivo principal (sem essa seção) com o do módulo (com ela).

![relação com o projeto pai](images/parent-in-pom-xml.png)