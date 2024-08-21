# davidjose4nb
Repositório 4NB
-----

# Análise de Requisitos - Módulo de Cadastro de Doações para ONG.

## 1. Descrição do Módulo

O módulo de cadastro de doações permite que doadores registrem suas doações, as quais são posteriormente direcionadas a ONGs específicas. O módulo também permite que os doadores acompanhem o destino e o status de suas doações.

## 2. Requisitos

### 2.1 Requisitos Funcionais
- **RF01:** Permitir o cadastro de doações com detalhes como tipo de doação (ex: alimentos, roupas), quantidade e informações do doador.
- **RF02:** Associar doações a ONGs específicas com base em critérios predefinidos (ex: necessidade da ONG, proximidade).
- **RF03:** Implementar uma funcionalidade para que o doador acompanhe o status e o destino de sua doação.
- **RF04:** Enviar notificações ao doador quando a doação for recebida pela ONG.
- **RF05:** Gerenciar o cadastro de ONGs participantes, incluindo detalhes como nome, localização e áreas de atuação.

### 2.2 Requisitos Não Funcionais
- **RNF01:** Interface amigável e acessível, com suporte para dispositivos móveis.
- **RNF02:** Tempo de resposta das operações (cadastro de doações, atualização de status) deve ser inferior a 3 segundos.
- **RNF03:** Suporte para até 5.000 doações ativas simultaneamente.

### 2.3 Regras de Negócio
- **RB01:** Doações não podem ser redirecionadas após terem sido designadas a uma ONG, a menos que autorizado pelo administrador.
- **RB02:** A ONG deve confirmar a recepção da doação antes de notificar o doador.
- **RB03:** Relatórios mensais devem ser gerados automaticamente, mostrando o número de doações e o total de recursos direcionados a cada ONG.

## 3. Análise de Viabilidade

- **Linguagem:** Utilizar Typescript para o desenvolvimento do backend.
- **Banco de Dados:** MySQL para armazenar dados das doações e informações das ONGs.
- **Infraestrutura:** Hospedagem em servidor com suporte para escalabilidade, visando o aumento de doações e ONGs no futuro.

## 4. Priorização dos Requisitos

### Método MoSCoW
- **Must Have:** Cadastro de doações, associação a ONGs, rastreamento do destino da doação, cadastro de ONGs.
- **Should Have:** Notificações automáticas para doadores.
- **Could Have:** Funcionalidade para doadores comentarem sobre sua experiência e interagirem com as ONGs.

---