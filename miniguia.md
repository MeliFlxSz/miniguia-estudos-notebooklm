## Resumo do Caso

Este estudo de caso analisa uma campanha de phishing que explora a popularidade do Claude para distribuir o malware PlugX (Remote Access Trojan - RAT). Os invasores utilizam engenharia social, typosquatting e um instalador aparentemente legítimo para comprometer o sistema da vítima. Após a instalação, o malware emprega técnicas de persistência, DLL sideloading e comunicação com um servidor de Comando e Controle (C2), permitindo acesso remoto ao computador e roubo de informações.

---

## Fluxo do Ataque

1. Criação de um site falso imitando o site oficial do Claude.
2. Download de uma falsa versão "Pro" do aplicativo.
3. Execução do instalador MSI.
4. Instalação do aplicativo legítimo para evitar suspeitas.
5. Execução do dropper em segundo plano.
6. Criação de persistência na inicialização do Windows.
7. Execução do PlugX utilizando DLL sideloading.
8. Comunicação com o servidor C2.
9. Roubo de informações e controle remoto da máquina.
10. Exclusão de vestígios da infecção.

---

## Glossário

| Conceito | Definição |
|----------|-----------|
| RAT | Malware que permite acesso remoto ao computador da vítima. |
| PlugX | Trojan de acesso remoto utilizado na campanha analisada. |
| Phishing | Técnica que busca enganar usuários para obter informações ou instalar malware. |
| Engenharia Social | Manipulação psicológica para induzir a vítima a realizar ações desejadas pelo invasor. |
| Typosquatting | Criação de domínios semelhantes aos originais para enganar usuários. |
| Dropper | Malware responsável por instalar a carga maliciosa principal. |
| DLL Sideloading | Técnica que faz um programa legítimo carregar uma DLL maliciosa. |
| Persistência | Mecanismo que mantém o malware ativo após reinicializações. |
| Payload | Carga maliciosa executada após a infecção. |
| C2 (Command and Control) | Servidor utilizado para controlar máquinas infectadas e receber dados roubados. |

---

## Principais Lições

- Verificar sempre o endereço do site antes de realizar downloads.
- Baixar softwares apenas de fontes oficiais.
- Desconfiar de versões não oficiais ou "Pro" oferecidas por terceiros.
- Manter soluções de segurança atualizadas.
- A engenharia social continua sendo um dos principais vetores de ataque.
- Ferramentas legítimas podem ser utilizadas para ocultar atividades maliciosas.

---

## Prompts Reutilizáveis

-explique o ataque, considerando que a explicação está sendo feita para uma pessoa que está começando a ter contato com cibersegurança e não conhece os conceitos e termos da área. Entretanto, apesar de ser iniciante em cibersegurança, a pessoa precisa entender de forma um pouco mais técnica e aprofundada, visto que ela é universitária de t.i. e ela precisa fazer uma apresentação desse estudo de caso, portanto não deve prevalecer simplificações e o uso de analogias durante todo o corpo do texto, sem esquecer de se apronfundar na explicação das terminologias próprias da área de cibersegurança. Quero que o formato da explicação demonstre o contexto anterior ao ataque e apresente a cronologia, exemplo: "contexto: '...' cronologia: 01/03/2026 -> explicação do acontecimento"

---

## Conclusão

Este estudo demonstrou como ataques modernos combinam engenharia social, ferramentas legítimas e técnicas avançadas de evasão para comprometer sistemas. A utilização do NotebookLM permitiu organizar as informações, aprofundar a compreensão do caso e produzir materiais de estudo reutilizáveis por meio da engenharia de prompts.
