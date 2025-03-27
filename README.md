# Rebolet0r

**⚠️ Projeto educacional e exclusivo para simulações em ambientes controlados e laboratórios. NÃO utilize este código para fins maliciosos.**

---

## 🧠 Visão Geral
O **Rebolet0r** é uma ferramenta de Red Team criada para demonstrar uma das técnicas de fraude bancária mais perigosas quando automatizada: o **reboletamento via IMAP**.

Inspirado em técnicas reais utilizadas por grupos criminosos, o Rebolet0r simula o comprometimento de contas de e-mail e a substituição de boletos legítimos por clones maliciosos com a mesma quantia, mas com código de barras e linha digitável redirecionados.

---

## ⚙️ Funcionalidades
- Conexão via IMAP com autenticação segura.
- Busca automatizada por e-mails com boletos (PDFs).
- Download e análise de PDFs anexados.
- Localização de elementos via coordenadas no plano cartesiano (linha digitável e código de barras).
- Geração de novos boletos via API bancária simulada.
- Substituição invisível do conteúdo PDF.
- Upload da nova versão para o mesmo e-mail, mantendo o header intacto.
- Notificação opcional via WhatsApp.
- Rastros temporários apagados com sobrescrita de arquivos (anti-forense).

---

## 📚 Arquitetura do Projeto
- **Linguagem:** C# (.NET Core)
- **IMAP:** MailKit
- **PDF Parsing:** PdfSharp
- **Leitura de Código de Barras:** IronBarCode (suporte ao padrão I-25 bancário)
- **Simulação bancária:** API REST 
- **Anti-forense:** Manipulação direta de arquivos `.eml` e sobrescrita de bytes antes da exclusão

---

## 🧪 Casos de Uso (LAB)
Este projeto é ideal para:
- Treinamentos de Red Team e Purple Team.
- Demonstrações em aulas sobre fraudes digitais.
- Desenvolvimento de contramedidas (Blue Team).
- Simulação de ataques avançados com foco em evasão de spam e detecção.

---

## 🚫 Importante
Este projeto **não será publicado em repositórios públicos** com código completo. As simulações devem ser feitas em ambientes de laboratório com e-mails controlados, como demonstrado no print do projeto.

Qualquer uso fora do contexto educacional é considerado crime, conforme o **Art. 154-A do Código Penal Brasileiro (Invasão de Dispositivo Informático)**.

---

## 👨‍🏫 Aula Sugerida
1. Introdução ao IMAP e técnicas de interceptação passiva.
2. Anatomia de um boleto bancário (código, linha digitável, padrões de barra).
3. Demonstração prática do Rebolet0r em ação (modo simulado).
4. Técnicas de defesa (MFA, análise comportamental, validação fora do e-mail).
5. Discussão sobre ética e legislação.

---

## 🙋‍♂️ Autor
Projeto criado por [Marcos Tolosa], profissional de segurança ofensiva especializado em automações de Red Team. Para saber mais ou convidar para treinamentos, entre em contato por DM.

---

## 🧠 Frase Final
> "A verdadeira segurança nasce quando entendemos o pensamento do atacante melhor do que ele mesmo."

---

**#RedTeam #CyberSecurity #Boletos #IMAP #FraudeFinanceira #EducaçãoDigital**

