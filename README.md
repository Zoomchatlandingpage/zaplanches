# ZapLanche — Demo comercial multiempresa

Protótipo navegável **sem backend e sem pagamentos reais**, destinado a apresentar o ZapLanche a trailers e lancheiros.

## Como experimentar
Abra o arquivo `index.html` em um navegador. Navegue entre Visão Geral, Estabelecimentos, Gestão Individual e Assinaturas. Selecione três estabelecimentos de exemplo, altere seus cardápios, cadastre equipe e motoboys e simule pedidos na Loja do cliente.

Os dados são mantidos somente na memória da página: ao atualizar, voltam ao estado inicial. Não há autenticação, PIX real, banco de dados ou proteção multiempresa implementada.

## Decisões de produto
- SaaS multiempresa com um painel Super Admin e painéis individuais futuramente.
- Administrador central pode editar a operação de cada trailer, mas **não valores efetivamente recebidos nem os dados de conta financeira**.
- Cada proprietário deverá controlar sua conta de recebimento PIX; pagamento real requer integração e validação segura por servidor.
- A demo tem 3 trailers fictícios e simulação de planos de 90 dias gratuitos seguidos de R$ 120/mês; essas condições vêm do PRD original.
- Os motoboys entram na demonstração comercial, embora sejam fase futura no PRD de operação.

## Próximas fases
1. Validar interface com comerciantes de Vitória da Conquista.
2. Refinar processo operacional e papéis de usuário.
3. Autenticação, banco de dados Supabase com isolamento RLS e trilha de auditoria.
4. Integração PIX com conta do comerciante, webhooks validados e reconciliação.
5. Deploy e testes de ponta a ponta.

**Atenção:** não utilizar este protótipo para vendas reais ou coleta de dados pessoais de clientes.
