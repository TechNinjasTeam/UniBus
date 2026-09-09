# UniBus

Marketplace que conecta operadores de transporte fretado universitário e alunos de outras cidades que estudam na Facens.

> `UniBus` é o nome de trabalho do projeto. Existem outros produtos com o mesmo nome no mercado; um eventual lançamento comercial passaria por rebranding.

## O problema

Quem depende de van ou ônibus fretado para chegar na faculdade vive um descompasso entre uma oferta rígida e uma demanda que muda todo dia. O operador sai com assento vazio ou deixa aluno na mão, e toda a comunicação acontece solta em grupos de WhatsApp: quem vai hoje, quem falta, a que horas é o retorno, onde a van está.

O UniBus organiza essa conversa em um fluxo só, com os dois lados no mesmo lugar.

## Como funciona

1. O operador cadastra a rota (cidade, faculdade, dias, horários de ida e volta, número de lugares) e os pontos de embarque com horário.
2. O operador gera um link de convite da rota e cola no grupo. O aluno entra por esse link já vinculado à rota.
3. Na ida vale o opt-out: todo mundo vai por padrão, quem avisa que não vai some da lista de embarque.
4. Na volta, o operador abre a chamada de retorno com hora limite de espera. O aluno confirma, e o operador acompanha ao vivo quem já respondeu.

## Funcionalidades

### Núcleo

**Operador**
- Cadastro de rota: cidade, faculdade, dias, horários de ida e volta, lugares
- Cadastro de pontos de embarque com horário
- Cadastro dos alunos que já atende e envio do link de convite
- Aprovação de solicitações de vaga
- Lista de embarque da ida, no modelo opt-out
- Chamada de retorno: hora limite de espera, ponto de onde a van está e checklist ao vivo de quem confirmou

**Aluno**
- Conta com e-mail, senha e telefone
- Entrada na rota pelo link de convite do operador; o vínculo com a lista do operador é feito pelo telefone
- Busca de rota por cidade e faculdade, com solicitação de vaga
- Consulta de ponto de embarque e horários
- Aviso de falta na ida
- Resposta à chamada de retorno

### Must have (Funcionalidades extra)

Previstas, ainda não implementadas:

- Notificação push, tela de instalação no iPhone e botão de copiar o link da chamada para o WhatsApp como plano B
- Check-in do operador no embarque
- Frequência por aluno e ocupação por viagem
- Controle de mensalidade (pago/pendente), marcado manualmente
- Localização da van em primeiro plano, com posição atualizada a cada ~10s e marcador que envelhece na tela do aluno

## Fora do escopo

Ficam para uma fase 2:

- Gateway de pagamento e cobrança automática da comissão
- Rastreamento em segundo plano (exige app nativo)
- App nativo / React Native
- Otimização de rota
- Chat entre operador e aluno
- Avaliação de motorista

## Modelo de receita

Comissão sobre a mensalidade paga pelo aluno ao operador. No MVP não há gateway de pagamento: a mensalidade é apenas marcada como paga ou pendente.


## Equipe

| Nome | Responsabilidade |
|------|-----------------|
| Gabriel Nunes Rodrigues| fundação e camada de dados |
| Alexander Da Silva Fernandes | telas do aluno|
| Moisés Ivanildo Ferreira | check-in, frequência e mensalidade|
| Maria Eduarda Fernandes Filhik | telas de rota, alunos e aprovação |


## Status

Em desenvolvimento.
