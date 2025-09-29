# Desafio de Projeto: Infraestrutura como Código com AWS CloudFormation

Este repositório documenta minha jornada ao concluir o desafio de **Infraestrutura como Código (IaC)**, uma proposta prática do bootcamp **Santander Code Girls**. O foco foi mergulhar no universo da AWS e automatizar o provisionamento de uma infraestrutura web simples utilizando **AWS CloudFormation**.

O grande objetivo? Sair da teoria e aplicar na prática a criação de recursos essenciais como instâncias EC2, servidores web e grupos de segurança, tudo definido em código através de templates `YAML`.

---

### O que eu aprendi com este desafio?

Ao final deste projeto, eu fortaleci e desenvolvi as seguintes habilidades:

- **Aplicar conceitos de IaC** em um ambiente real na AWS, saindo do manual para o automatizado.
- **Criar e gerenciar Stacks (Pilhas)** no CloudFormation, entendendo seu ciclo de vida.
- **Estruturar templates em YAML** para definir recursos de nuvem de forma declarativa e versionável.
- **Automatizar a configuração de software** em instâncias EC2 com scripts de `UserData`, tornando o setup mais inteligente.
- **Documentar processos técnicos** de forma clara e estruturada (como este README!).
- **Utilizar o GitHub** como ferramenta central para compartilhar e versionar a documentação e os templates do projeto.

---

### 🛠️ Minha Jornada Prática: Execução e Evidências

A prática foi dividida em três experimentos principais, onde cada um adicionava uma camada de complexidade. Para cada etapa, eu criei uma **Stack** independente no CloudFormation, fazendo o upload do template `YAML` correspondente.

#### 1. Experimento: `laboratorio-ec2`
- **Objetivo:** O primeiro passo! Criar uma instância EC2 simples, sem configurações extras, apenas para validar o fluxo básico de provisionamento e entender como uma Stack se comporta.
- **Resultado:** Sucesso! A pilha `laboratorio-ec2` foi criada com o status `CREATE_COMPLETE`, confirmando que o CloudFormation provisionou a instância EC2 conforme o esperado. Missão cumprida!

#### 2. Experimento: `lab-apache`
- **Objetivo:** Ir além. Provisionar uma instância EC2 e, de forma 100% automatizada, instalar e configurar um servidor web Apache usando a seção `UserData` do template.
- **Resultado:** A pilha `lab-apache` subiu perfeitamente. O template `YAML` continha os comandos para instalar, iniciar e habilitar o serviço Apache, além de criar uma página `index.html` de boas-vindas. O resultado foi uma instância EC2 pronta para servir conteúdo web assim que foi criada.

#### 3. Experimento: `lab-firewall`
- **Objetivo:** Unificar tudo. Criar uma instância EC2 que já instala o servidor web e, ao mesmo tempo, define seu próprio **Grupo de Segurança (Security Group)** para liberar o tráfego na porta 80 (HTTP).
- **Resultado:** Este foi o experimento que conectou tudo. A pilha `lab-firewall` demonstrou o verdadeiro poder da IaC ao provisionar a instância `WebserverFirewall` e o firewall necessário para ela em uma única operação. Tudo atômico, tudo conectado.

---

### 💡 Minhas Impressões e Conclusão

Este desafio foi um divisor de águas para solidificar meu entendimento sobre **Infraestrutura como Código**.

A maior lição que tirei foi perceber como é poderoso criar, replicar e destruir ambientes inteiros de forma rápida, consistente e, o mais importante, **livre de erros manuais**. O CloudFormation abstrai a complexidade do console da AWS e garante que a infraestrutura implantada seja exatamente aquela declarada no código.

Começar com uma stack simples e evoluir para uma que combina múltiplos recursos interconectados abriu minha mente para a criação de **templates reutilizáveis e modulares**. Sinto que agora tenho a base necessária para construir arquiteturas mais complexas e robustas na nuvem.

---

### Autora

**Julia Krisnarane**

- **LinkedIn:** [linkedin.com/in/SEU-PERFIL](https://www.linkedin.com/in/julia-krisnarane-moraes-410417345)
- **GitHub:** [github.com/SEU-USUARIO](https://github.com/krisnarane)
