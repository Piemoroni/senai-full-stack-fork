# Estacionamento Pro - Sistema de Gestão

Sistema web para controle de fluxo de veículos em estacionamentos, permitindo o cadastro detalhado de frotas e o monitoramento de tempo de permanência com cálculo automático de valores.

## Demonstração (Screenshots)

| Tela Inicial | Cadastro de Veículos |
|---|---|
| ![tela1](./img/home.png) | ![tela2](./img/cadastro.png) |

| Cadastro de Estadias | Estadia em Andamento |
|---|---|---|
| ![tela3](./img/estadia.png) | ![tela4](./img/andamento.png) | 

| Estadia Finalizada |
|---|
|![tela5](./img/finalizada.png) |

---

## Funcionalidades

- **Módulo de Veículos**:
  - Cadastro completo seguindo rigorosamente os requisitos da API.
  - Listagem de veículos com visualização de proprietário e marca.
  - Exclusão de veículos cadastrados.
- **Módulo de Estadias**:
  - Registro de entrada vinculada à placa.
  - Botão de **Finalizar** direto no card (registra saída e calcula valor).
  - Diferenciação visual: Estadias finalizadas ficam em **azul**.
  - Exclusão de registros de histórico.

## Especificações Técnicas

### Estrutura do Objeto (Veículo)
O sistema envia os dados para o Back-end exatamente neste formato:
```json
{
  "placa": "AAA2222",
  "proprietario": "Pietra Moroni",
  "tipo": "Carro",
  "modelo": "Pulse",
  "marca": "Fiat",
  "cor": "Cinza Escuro",
  "ano": 2022,
  "telefone": "11 89563201"
}