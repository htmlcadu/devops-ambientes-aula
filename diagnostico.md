**Etapa 3 (Parte A) – Diagnóstico, camadas afetadas e classificação das intervenções**

| Problema | Consequência | Estado desejado | Evidência da correção | Camadas e intervenção |
|---|---|---|---|---|
| Versões de banco diferentes em homologação e produção | Homologação não representa produção; falhas só aparecem com usuários reais | Mesma versão, definida em código versionado | Código com versão única; consulta de versão igual nos dois bancos | Banco de dados e ambientes. Provisionamento, configuração e implantação |
| Porta liberada manualmente | Exposição sem registro nem revisão; ambiente difícil de reproduzir | Portas necessárias declaradas no código e revisadas | Regra no repositório; plan ou `--check --diff` sem diferenças | Rede e segurança. Configuração e gerenciamento |
| Configuração dependente de uma pessoa | Ponto único de falha; difícil recuperar o ambiente | Configuração versionada, revisada e reproduzível por qualquer integrante | Recriar o ambiente a partir do repositório | Processo e equipe. Gerenciamento |
