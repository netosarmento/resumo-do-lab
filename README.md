# resumo-do-lab
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO
## Resumo | 1
- O azure, cloud da Microsoft. Contem um painel me simples e facil de utilizar com os termos já conhecidos, sem inventar nomes. Facil para locarlizar seus serviços e configurações.
- Mostrou os serviços, de Maquina virtuais. Configurações de gateway e firewall.
- utilização de chave ssh.
- Utilização de jump serv, além de demonstrar o tradicional windows server entre outros.
- Zonas de DNS, balançeadores de carga.
- Criação de imagens, emparelhamento de redes, e armazenamento.

## Resumo | 2
- Criação de VM na Azure
### Os benefícios
- Escalabilidade e elasticidade 
- Confiabilidade, previsibilidade e segurança 
- Governança e Gerenciabilidade

## Resumo | 3
- Modelos de Serviços
### IaaS,PaaS,SaaS

- IaaS : Infraestrutura como serviço, mais nossas (Dev) responsabilidade.

- PaaS : Plataforma como serviço, ambas responsabilidade. 

- SaaS : Software como serviço. menos responsabilidade.

## Resumo | 4

Arquitetura:
- Alta disponibilidade
- Pares de regiões para, manter disponibilidade.
- Conjunto de disponibilidade, domínio de atualizações e domínio de falhas.
- Recuperação automática mas somente para alguns serviços.
- Zonas de disponibilidade possibilita, alta disponibilidade e baixa latência.
- regiões soberanas:
- Azure EUA - área militar 
- Azure China - Operado pela 21vianet
- Datacenters
- Grupo de recursos, escolher recursos e região
- Conta Azure:
- Assinaturas
- Desenvolvimento, Teste e Produção
- Grupos de gerenciamento das assinaturas.

Site infraestrutura Azure:
https://azure.microsoft.com/en-us/explore/global-infrastructure

## Resumo | 5

Rede de computação
 
- serviços de computação e VM Azure
- Conjunto de disponibilidade de VM
- Domínio de falhas / Domínio de atualização (Configuração s/ custo)
- Área de trabalho virtual do Azure ( Virtualização de um desktop )
- Serviço de Contêineres ( Docker ) : Azure ( Modelo: PaaS )
- Aplicativos de Contêineres do Azure : Uma oferta de PaaS, como instância de Contêineres, que pode balancear carga e escalar.
- Serviço de Kubernetes do Azure: um serviço de orquestração para contêineres com arquitetura distribuídas e grandes volumes de Contêineres. ( AKS )
- Azure Functions: Uma oferta de PaaS, que dá suporte a operações de computação sem servidor.
- Um código baseado em eventos, é executado quando chamado, sem exigir infraestrutura de um servidor quando inativo.
- Migrações: Lift-and-Shift ( Levar como está )
- Serviços Aplicativos Azure : .NET, .NET core, Node.js, Java, PhP e Python. ( Linguagens )
- Oferta de PaaS com requisito de nível corporativo de desempenho, segurança e conformidade. ( PaaS: pois não tem sistema operacional envolvo, os aplicativos web )
- Rede Virtual Azure ; VNet :
- Pontos de Extremidades públicos, acessível de qualquer lugar.
- Pontos de Extremidades privados, acessível somente pela nossa rede.
- VPN Azure
- ExpressRoute Azure : Feito via cabos
- DNS Azure
- VM e contêineres são isolados do hardwares e do host.
- Famílias de VM's : LAMP stack using Azure VM, Scalable WordPress using Azure VM, VM Starter Kit Linux.
- Para possibilitar comunicação entre redes virtuais é necessário emparelhamento de redes.

## Resumo | 6

Armazenamento:

- Azcopy: Gerenciar armazenamento.
- Sincronização de arquivos Azure
- Migrações 
- Azure DataBox
- Configurações de redundância 
- LRS ( Armazenamento com redundância local ) : Implementação: data center individual na região primária / 11 noves
- ZRS ( Armazenamento com redundância na zona ) : Implementação: Três zonas de disponibilidade na região primária / 12 noves
- GRS ( Armazenamento com redundância geografica ) : Implementação: Data Center único  região primária e secundária / 16 noves
- ZGRS ( Armazenamento com redundância na zona geografica ) : Implementação: Três zonas de disponibilidade na região primária e Data Center único  região secundária / 16 noves
- Pontos de Extremidades públicos, de Armazenamento.
- Armazenamento blog, Data Lake, Armazenamento Azure, Armazenamento filas, Armazenamento em tabelas.
- Camadas de acesso.
- Frequente / Esporádico / Frio / Arquivo morto
- Azure DataBox comporta até 80 TB
- DataBox Disk / DataBox / DataBoxHeavy ( Caminhão )
- Conectar o Storage account :
- Verificar letra de unidade 
- Métodos de Autenticação 
- Chave da conta de armazenamento 
- Activety direct no Microsoft
- Protocolo SMB porta 445

## Resumo | 7

Identidade, acesso e segurança: domínio e objetivo 

- Conceito de confiança zero

- Finalidade de um Modelo de defesa em profundidade 

- Descrever finalidade do Microsoft defender pra nuvem 

- Microsoft entra id ( Active Directory )

- Logon único ( SSO )

- Negócios para negócios ( B2B )

- Gerenciamento de aplicativos e dispositivos 

- Autenticação MFA

Acesso Condicional:

- Associação de um usuário ao grupo 

- Local do IP

- Dispositivo

- Aplicativo 

- Detecção de riscos

## Resumo| 8

Gerenciamento de custos :

- TCO ( Calculadora Total de Propriedade )
- Custos e Previsibilidade de valores 
- TCO : https://azure.microsoft.com/en-us/pricing/tco/calculator/
- Calculadora de Preço : https://azure.microsoft.com/en-us/pricing/calculator/
- Diferentes estratégias para utilizar VM's  
- Pagar por uso / Reserva / modelo híbrido / diminuir tempo útil.

## Resumo| 9

Governança e Confirmadade: 

- Blueprints, Políticas e Bloqueio de recursos.
- Azure Policy : Políticas de padrões organizacionais para conformidade em escala.
- Ele fornece governança e consistência de recursos com conformidade regulatória, segurança, custo e gerenciamento.
- Bloqueio de Recursos :
- Proteja os recursos do Azure, de ser deletado ou modificado acidentalmente .
- Microsoft Purview.
- Portalde Confiança do serviço.

Ferramentas de Implementação de Recursos:

- PowerShell, CLI, portal
- Azure Arc e Azure Resources Manage.
- Bícep ( Linguagem Cloud Microsoft )
- Azure Resource Manager ( Json )