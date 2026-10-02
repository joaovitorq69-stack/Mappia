# Mappia

Documento de requisitos do produto (PRD)

Versão 3.0 | 02/10/2026

Projeto de extensão de Ciência da Computação da UNINASSAU Campina Grande, na disciplina Atividades Práticas Interdisciplinares de Extensão I.

## Equipe

- [João Vitor Regis](https://github.com/joaovitorregis)
- [Ryan Cavalcante](https://github.com/Ryancscarvalho)
- [Joalison Normandia](https://github.com/joalisonnormandia)
- [Jhonatan Xavier](https://github.com/jhonatandevpb)


## 1. Visão do produto

O Mappia é uma proposta de plataforma web para registrar problemas urbanos, consultar sua localização e acompanhar o andamento de cada ocorrência. O uso prioriza o celular. O registro pode ser enviado sem conta; o cadastro é oferecido depois, para reunir os registros do morador.

O bairro das Malvinas, em Campina Grande (PB), é a área prevista para o piloto. O projeto está em fase de protótipo e planejamento. Os requisitos deste PRD descrevem o produto previsto, sem indicar que suas funções já estejam implementadas.

## 2. Objetivos

O objetivo principal é reunir registros de problemas urbanos em um mapa e permitir seu acompanhamento por protocolo. A equipe revisa as informações antes de sua divulgação pública.

Os objetivos de evolução incluem mapear pontos de descarte de resíduos, divulgar comércio local, registrar doações e voluntariado, publicar alertas comunitários e apoiar o encaminhamento das ocorrências aos órgãos responsáveis. Esses recursos têm prioridades S ou C no backlog.

## 3. Perfis de uso

| Perfil | Acesso previsto |
| --- | --- |
| Visitante | Mapa público, envio sem conta e consulta por protocolo. |
| Morador com conta | Registros vinculados à conta; recursos adicionais de acesso e avisos nas evoluções previstas. |
| Equipe de moderação | Acesso restrito para validar, rejeitar e alterar estados. |
| Comerciante | Conta para cadastrar estabelecimento, após o MVP (7.1). |
| Liderança comunitária | Consulta pública e futura exportação de resumos (6.3). |
| Órgão responsável | Destinatário do encaminhamento previsto em 5.6; sem painel próprio no MVP. |

## 4. Prioridades e entregas

M significa essencial para o MVP; S identifica evoluções importantes; C identifica evoluções desejáveis. Os pontos são estimativas relativas de esforço, não horas de trabalho nem datas de entrega.

O MVP reúne os 30 itens M, com 96 pontos. A entrega inclui registro sem conta, protocolo, cadastro opcional, mapa, acompanhamento, moderação, indicadores e base técnica. A moderação e as regras de acesso fazem parte do MVP.

As evoluções S e C permanecem no planejamento. O aplicativo nativo, a integração automática com sistemas internos da prefeitura, a moderação por IA e pagamentos estão fora do escopo documentado.

| Épico | Tema | M | S | C |
| --- | --- | --- | --- | --- |
| 1 | Denúncia sem cadastro | 19 | 10 | 0 |
| 2 | Cadastro opcional após o envio | 9 | 8 | 3 |
| 3 | Mapa colaborativo | 13 | 8 | 2 |
| 4 | Acompanhamento | 6 | 9 | 3 |
| 5 | Prevenção de abuso e moderação | 17 | 12 | 0 |
| 6 | Painel de indicadores | 3 | 3 | 5 |
| 7 | Recursos da comunidade | 0 | 8 | 13 |
| 8 | Base técnica e entrega | 29 | 3 | 0 |
|  | Total | 96 | 61 | 26 |

## 5. Requisitos funcionais

Cada grupo corresponde ao épico de mesmo número no Product Backlog. Os IDs identificam os requisitos nas duas versões.

### RF1. Denúncia sem cadastro

| ID | Requisito | Prioridade | Pontos |
| --- | --- | --- | --- |
| 1.1 | Acessar o formulário sem conta | M | 2 |
| 1.2 | Selecionar a categoria | M | 2 |
| 1.3 | Descrever o problema | M | 1 |
| 1.4 | Informar a localização por mapa ou GPS | M | 5 |
| 1.5 | Anexar foto do problema | M | 5 |
| 1.6 | Exibir aviso de privacidade antes do envio | M | 2 |
| 1.7 | Confirmar o envio e gerar protocolo | M | 2 |
| 1.8 | Avisar sobre possível duplicata | S | 5 |
| 1.9 | Confirmar Também vejo esse problema | S | 3 |
| 1.10 | Remover metadados EXIF da foto | S | 2 |

### RF2. Cadastro opcional após o envio

| ID | Requisito | Prioridade | Pontos |
| --- | --- | --- | --- |
| 2.1 | Oferecer cadastro após confirmar o registro | M | 3 |
| 2.2 | Dispensar o cadastro | M | 1 |
| 2.3 | Criar conta e vincular o registro atual | M | 5 |
| 2.4 | Vincular registros anteriores do aparelho | S | 3 |
| 2.5 | Consultar registros em outro aparelho | S | 3 |
| 2.6 | Recuperar senha por e-mail | S | 2 |
| 2.7 | Entrar por link enviado ao e-mail | C | 3 |

### RF3. Mapa colaborativo

| ID | Requisito | Prioridade | Pontos |
| --- | --- | --- | --- |
| 3.1 | Exibir ocorrências no mapa público | M | 5 |
| 3.2 | Distinguir os estados das ocorrências | M | 2 |
| 3.3 | Abrir o detalhe de uma ocorrência | M | 3 |
| 3.4 | Filtrar o mapa por categoria | M | 3 |
| 3.5 | Buscar rua ou ponto de referência | S | 3 |
| 3.6 | Exibir camadas temáticas | S | 5 |
| 3.7 | Agrupar pinos próximos | C | 2 |

### RF4. Acompanhamento

| ID | Requisito | Prioridade | Pontos |
| --- | --- | --- | --- |
| 4.1 | Consultar pelo protocolo sem conta | M | 3 |
| 4.2 | Listar os registros da conta | M | 3 |
| 4.3 | Copiar link de uma ocorrência | S | 1 |
| 4.4 | Consultar histórico de estados | S | 3 |
| 4.5 | Receber aviso de mudança de estado | S | 5 |
| 4.6 | Sugerir resolução com foto | C | 3 |

### RF5. Prevenção de abuso e moderação

| ID | Requisito | Prioridade | Pontos |
| --- | --- | --- | --- |
| 5.1 | Verificar envios contra robôs | M | 3 |
| 5.2 | Limitar a frequência de envios | M | 3 |
| 5.3 | Restringir o acesso da equipe | M | 3 |
| 5.4 | Validar ou rejeitar a ocorrência | M | 5 |
| 5.5 | Alterar o estado de uma ocorrência | M | 3 |
| 5.6 | Encaminhar ao órgão responsável | S | 5 |
| 5.7 | Sinalizar conteúdo falso ou ofensivo | S | 2 |
| 5.8 | Unir registros duplicados | S | 3 |
| 5.9 | Ocultar dados pessoais em fotos | S | 2 |

### RF6. Painel de indicadores

| ID | Requisito | Prioridade | Pontos |
| --- | --- | --- | --- |
| 6.1 | Contar ocorrências validadas por estado | M | 3 |
| 6.2 | Apresentar categorias mais frequentes | S | 3 |
| 6.3 | Exportar resumo em PDF ou CSV | C | 5 |

### RF7. Recursos da comunidade

| ID | Requisito | Prioridade | Pontos |
| --- | --- | --- | --- |
| 7.1 | Cadastrar estabelecimento comercial | S | 5 |
| 7.2 | Mapear pontos de descarte de resíduos | S | 3 |
| 7.3 | Publicar alertas comunitários | C | 5 |
| 7.4 | Registrar doações e voluntariado | C | 8 |

### RF8. Base técnica e entrega

| ID | Requisito | Prioridade | Pontos |
| --- | --- | --- | --- |
| 8.1 | Levantar dados e definir categorias | M | 5 |
| 8.2 | Preparar protótipo navegável | M | 3 |
| 8.3 | Configurar serviços Firebase | M | 5 |
| 8.4 | Aplicar regras de acesso aos dados | M | 3 |
| 8.5 | Implementar interface responsiva | M | 3 |
| 8.6 | Documentar privacidade e termos de uso | M | 2 |
| 8.7 | Realizar teste de usabilidade com moradores | M | 5 |
| 8.8 | Corrigir problemas do teste | M | 3 |
| 8.9 | Divulgar o projeto | S | 3 |

## 6. Fluxo e regras de negócio

O fluxo principal parte do mapa, segue para Reportar problema e para o formulário, e termina com a confirmação e o protocolo. Depois do envio, o visitante pode criar conta ou continuar sem cadastro. A consulta por protocolo permanece disponível nos dois casos.

- O visitante acessa o mapa, registra uma ocorrência e consulta o protocolo sem criar conta.
- O convite de cadastro aparece após a confirmação. Dispensar o convite não apaga o registro.
- Cada envio persistido recebe um protocolo único e começa em Em análise.
- A equipe valida o registro como Pendente ou Crítico, ou o classifica como Rejeitado. Uma ocorrência validada pode passar a Resolvido.
- O mapa e os indicadores públicos usam apenas ocorrências validadas. Em análise e Rejeitado ficam fora das contagens públicas.
- A consulta por protocolo permite acompanhar o registro sem expor dados privados do autor. O protocolo não dá permissão para editar, moderar ou vincular um registro a uma conta.
- O registro recém-enviado é vinculado à conta criada na mesma sessão. O vínculo de registros anteriores do aparelho é uma evolução prevista no item 2.4.
- Contas da equipe exigem autenticação e permissão administrativa. O cadastro de comerciantes, previsto após o MVP, também exige conta.
- A classificação Crítico indica prioridade da ocorrência. Ela não representa um acionamento de emergência ou garantia de atendimento.
- O encaminhamento a órgãos responsáveis é uma evolução do item 5.6. O registro não garante atendimento ou resolução pelo poder público.

As categorias iniciais são buraco, iluminação, lixo, vazamento, acessibilidade e sinalização (1.2 e 8.1). Qualquer alteração no catálogo precisa manter formulário, filtro e documentos consistentes.

## 7. Dados e arquitetura prevista

A base técnica prevista usa HTML, CSS e JavaScript na interface, Leaflet no mapa e Firebase para autenticação, banco de dados e imagens. São escolhas de planejamento dos itens 3.1 e 8.3; não descrevem serviços já implantados.

| Dado | Uso previsto |
| --- | --- |
| Protocolo | Identificador único para acompanhamento. |
| Categoria e descrição | Classificação e relato do problema. |
| Latitude e longitude | Localização indicada no mapa ou obtida por GPS autorizado. |
| Foto | Imagem associada ao relato, submetida à revisão antes da divulgação. |
| Estado e datas | Estado atual, criação e atualização; histórico detalhado previsto em 4.4. |
| Identificador de sessão ou conta | Associação interna ao envio e posterior vínculo com conta; não aparece no mapa público. |
| Validação | Decisão da equipe e conteúdo liberado para consulta pública. |
| Confirmações e encaminhamento | Dados das evoluções 1.9 e 5.6, após o MVP. |

O acesso público deve ser separado dos dados privados e das operações administrativas (8.4). Antes da validação, a ocorrência permanece na fila da equipe; o autor acompanha seu estado pelo protocolo.

## 8. Requisitos não funcionais

| Área | Requisito e vínculo com o backlog |
| --- | --- |
| Privacidade | Aviso antes do envio (1.6), acesso restrito aos dados privados (8.4) e política de privacidade (8.6). Fotos inadequadas ficam fora da divulgação durante a revisão (5.4). A remoção automática de EXIF (1.10) e a ferramenta de ocultação de dados em imagens (5.9) são evoluções S. |
| Controle de acesso | Verificação antiabuso e limite de envios (5.1 e 5.2); autenticação e autorização da equipe (5.3); regras de leitura e escrita (8.4). |
| Usabilidade | Formulário curto, linguagem simples, rótulos claros e estados identificados por texto e cor. Os testes com moradores fazem parte da entrega (8.7 e 8.8). |
| Compatibilidade | Interface web responsiva com prioridade para celular (8.5), sem instalação de aplicativo nativo. |
| Desempenho | Fotos e mapa precisam permitir uso em conexão móvel. Agrupamento de pinos permanece como evolução C (3.7). |
| Manutenção | Código versionado e documentação das configurações de autenticação, categorias, estados e acesso aos dados (8.3 e 8.4). |

## 9. Avaliação prevista

| Indicador | Medição | Meta proposta |
| --- | --- | --- |
| Tempo de envio | Tempo para concluir um registro no teste de usabilidade. | Até 2 minutos. |
| Conclusão do fluxo | Proporção de participantes que concluem sem ajuda. | Pelo menos 80%. |
| Satisfação | Questionário SUS após as tarefas do teste. | Pontuação de pelo menos 70. |
| Prazo de análise | Tempo entre envio e decisão da equipe durante o piloto. | Até 48 horas como meta do piloto. |
| Qualidade dos registros | Proporção de rejeitados e duplicados. | Acompanhar a evolução, sem meta numérica definida. |
| Adoção da conta opcional | Contas criadas em relação aos registros enviados. | Medir sem meta fixa. |

Essas metas são propostas de avaliação, não resultados obtidos ou garantia de serviço. O item 8.7 registra as medições e o item 8.8 trata as dificuldades observadas.

## 10. Sequência de implementação

A sequência parte da preparação e da base técnica (8.1 a 8.6), integra mapa e registro, conecta acompanhamento e conta opcional, e fecha a entrega com moderação, indicadores, testes e ajustes. Não há datas de sprints ou responsáveis por tarefa definidos nesta revisão.

O MVP só está completo quando todos os itens M atendem aos critérios do backlog. As evoluções S e C não substituem itens M pendentes. Protótipo visual e implementação funcional têm avaliações distintas.

## 11. Dependências e limites de operação

A publicação do serviço depende da definição do ambiente de hospedagem, dos limites de armazenamento, da política de retenção e exclusão de dados e da rotina de moderação. O encaminhamento futuro depende da escolha de um canal para o órgão responsável. Nenhuma parceria institucional ou integração com a prefeitura é presumida.

Envios abusivos, exposição indevida em fotos, baixa participação e carga de moderação são riscos do produto. Os itens 5.1, 5.2, 5.4, 8.4, 8.6, 8.7 e 8.8 tratam a primeira entrega; 1.10, 5.7, 5.8 e 5.9 acrescentam controles na evolução.

## 12. Documentos relacionados

- [Product Backlog do Mappia, versão 3.0](../product-backlog/Product_Backlog_Mappia.md)
- [Protótipo no Figma](https://www.figma.com/design/IY3T4Dv7QenJZWPRxngnf3)

## Histórico da revisão

Versão 3.0, 02/10/2026: nomenclatura Mappia nos dois documentos; requisitos ligados aos mesmos 55 IDs; preservação das prioridades e dos pontos do backlog anterior; critérios de aceitação detalhados. Encaminhamento, privacidade das imagens e publicação de estados têm a mesma fase de entrega no PRD e no backlog.
