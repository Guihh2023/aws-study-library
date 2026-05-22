# 🔐 Modelo de Responsabilidade Compartilhada (AWS)

O modelo de responsabilidade compartilhada define o que é responsabilidade da AWS e o que é responsabilidade do cliente ao usar serviços em nuvem.

---

# ☁️ O que é?

É um modelo que divide a segurança e gestão da nuvem entre:

- AWS (provedor da nuvem)
- Cliente (usuário da nuvem)

---

# 🏢 Responsabilidade da AWS

A AWS é responsável pela **segurança da nuvem**.

Ela cuida de:

- Infraestrutura física (data centers)
- Hardware (servidores, storage, rede)
- Virtualização
- Segurança dos datacenters
- Disponibilidade da infraestrutura

---

# 👤 Responsabilidade do Cliente

O cliente é responsável pela **segurança dentro da nuvem**.

Inclui:

- Controle de acesso (IAM)
- Configuração de serviços (EC2, S3, etc.)
- Dados armazenados
- Sistema operacional (em serviços IaaS)
- Criptografia e permissões

---

# ⚖️ Como funciona na prática?

Depende do tipo de serviço:

## 🏗️ IaaS (ex: EC2)

Você gerencia quase tudo:
- sistema operacional
- aplicações
- dados
- firewall (Security Groups)

AWS gerencia a infraestrutura física.

---

## ⚙️ PaaS (ex: Lambda)

AWS gerencia mais coisas:
- infraestrutura
- sistema operacional
- runtime

Você gerencia apenas:
- código
- dados

---

## 📦 SaaS (ex: Gmail)

AWS (ou provedor) gerencia tudo.

Você só usa o sistema.

---

# 📊 Diagrama mental simples

- AWS → segurança da infraestrutura
- Cliente → segurança do uso e configuração

---

# 🚨 Erros comuns

- Achar que AWS cuida de tudo automaticamente
- Não configurar permissões corretamente no IAM
- Deixar buckets S3 públicos sem querer
- Não proteger dados sensíveis

---

# 🧠 Exemplo prático

Se você cria uma instância EC2:

- AWS garante que o servidor físico existe e está funcionando
- Você precisa:
  - configurar o sistema operacional
  - instalar aplicações
  - proteger o acesso

---

# 🔥 Resumo rápido

O modelo de responsabilidade compartilhada define:

👉 AWS cuida da infraestrutura  
👉 Cliente cuida da configuração e segurança dos dados

---

# 🎯 Importância

Esse conceito é fundamental para:

- Segurança na AWS
- Certificações
- Entrevistas de Cloud
- Boas práticas de arquitetura
