# pgats-ci-challenge01
```
exercício 03
Leia sobre self-hosted runners/agents. Avalie: Quando faz sentido usar esse recurso? Outras plataformas oferecem recursos similares? Implemente um self-hosted agent para executar sua pipeline.
```

## Vantagens
* **Redução de custos**: Sem cobrança por minuto de execução, ideal para fluxos longos ou pesados.
* **Hardware customizado**: Permite escolher a quantidade exata de CPU, RAM, armazenamento e uso de GPUs.
* **Acesso à rede interna**: Conecta-se diretamente a bancos de dados e servidores privados sem expor portas à internet.
* **Sem limites de tempo**: Execuções podem durar mais do que o limite padrão de 6 horas do GitHub.
* **Pré-configuração**: Ferramentas e dependências grandes podem ficar pré-instaladas para acelerar o build.

## Desvantagens
* **Custos de infraestrutura**: Exige pagar pelos servidores, armazenamento e transferência de dados da sua própria nuvem.
* **Sobrecarga de manutenção**: Sua equipe precisa gerenciar atualizações do sistema operacional, segurança e patches do runner.
* **Riscos de segurança**: Repositórios públicos usando self-hosted runners podem sofrer ataques de execução de código malicioso.
* **Escalabilidade manual**: Você precisa configurar o auto-scaling para lidar com picos de builds simultâneos.
* **Isolamento de ambiente**: Builds subsequentes podem herdar arquivos residuais se o ambiente não for limpo adequadamente.

## Quando escolher cada opção
* **Self-Hosted**: Você tem fluxos de CI/CD que duram horas, precisa implantar em uma VPC privada, ou exige hardware específico (como GPUs para Machine Learning).
* **GitHub-Hosted**: Você quer foco total no desenvolvimento, possui projetos de código aberto (open-source) ou tem fluxos de trabalho leves e padronizados.