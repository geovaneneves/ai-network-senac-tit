# Guia de Importação da Máquina Virtual Ubuntu Server 22.04.4 LTS no Oracle VirtualBox 7.2

## Objetivo
Importar a imagem **UbuntuServer-OnPremises.ova** disponibilizada pelo Professor Robson Vaamonde e configurar a rede em **Modo Bridge (Ponte)** utilizando a rede cabeada do laboratório (**10.24.82.0/24**).

---

# 🖥️ Pré-requisitos

Antes de iniciar, confirme que:

✅ Oracle VirtualBox 7.2 instalado

✅ Arquivo `UbuntuServer-OnPremises.ova` disponível na pasta **Downloads**

✅ Computador conectado à rede cabeada do laboratório

✅ Sistema Operacional Windows 11

✅ Permissões para executar o VirtualBox

---

# 📥 Etapa 1 - Abrir o Oracle VirtualBox

1. Clique no menu **Iniciar** do Windows.
2. Digite **VirtualBox**.
3. Clique em **Oracle VirtualBox**.

📌 Aguarde a abertura da tela principal.

---

# 📦 Etapa 2 - Importar a Máquina Virtual

1. Na barra superior clique em:

   **Arquivo → Importar Appliance**

2. Clique no ícone 📁 **Escolher Arquivo**.

3. Navegue até:

   ```
   Downloads
   ```

4. Selecione o arquivo:

   ```
   UbuntuServer-OnPremises.ova
   ```

5. Clique em **Próximo**.

---

# ⚙️ Etapa 3 - Revisar Configurações da Importação

Será exibida uma tela com as configurações da máquina virtual.

Verifique:

- Nome da VM
- Quantidade de memória
- CPUs virtuais
- Controladoras de disco
- Adaptadores de rede

📌 Normalmente não é necessário alterar nenhuma configuração.

Clique em:

**Finalizar**

---

# ⏳ Etapa 4 - Aguardar a Importação

O VirtualBox iniciará a importação da imagem.

Dependendo do desempenho do equipamento:

⏱️ Tempo médio: 2 a 10 minutos

Ao finalizar, a máquina virtual aparecerá no painel esquerdo do VirtualBox.

---

# 🌐 Etapa 5 - Configurar Rede em Modo Bridge (Ponte)

## Selecionar a Máquina Virtual

1. Clique sobre:

   ```
   UbuntuServer-OnPremises
   ```

2. Clique em:

   **Configurações** ⚙️

---

## Acessar Rede

1. Clique na opção:

   **Rede**

2. Verifique se:

   ☑ Habilitar Placa de Rede

está marcado.

---

## Alterar para Bridge

Em:

**Conectado a:**

Selecione:

```text
Placa em Modo Bridge (Adaptador em Ponte)
```

---

## Escolher a Interface Física

Em:

**Nome:**

Selecione a placa de rede cabeada do laboratório.

Exemplos:

```text
Intel Ethernet Controller
Realtek PCIe GbE Family Controller
Intel I219-V
```

⚠️ Não selecionar interfaces Wi‑Fi ou virtuais.

Utilize a interface Ethernet física conectada ao switch da sala.

---

## Confirmar Configuração

Clique em:

**OK**

para salvar as alterações.

---

# ▶️ Etapa 6 - Inicializar a Máquina Virtual

1. Selecione a VM.
2. Clique em:

   **Iniciar** ▶️

3. Aguarde o carregamento do Ubuntu Server.

---

# 🔍 Etapa 7 - Verificar Configuração de Rede

Após realizar login:

Execute:

```bash
ip addr
```

ou

```bash
ip a
```

Verifique se a interface recebeu um endereço IP da rede:

```text
10.24.82.x
```

Exemplo:

```text
10.24.82.150/24
```

---

# 📡 Etapa 8 - Testar Comunicação com a Rede

Teste conectividade executando:

```bash
ping 10.24.82.1
```

ou o gateway informado pelo instrutor.

Para interromper:

```bash
Ctrl + C
```

---

# 🌍 Etapa 9 - Testar Acesso à Internet

Execute:

```bash
ping google.com
```

Resultado esperado:

```text
64 bytes from ...
```

Caso responda corretamente, a conectividade está funcionando.

---

# ✅ Checklist Final

Verifique:

☑ Arquivo OVA importado com sucesso

☑ Máquina virtual criada no VirtualBox

☑ Adaptador configurado em Bridge (Ponte)

☑ Interface Ethernet física selecionada

☑ VM inicializada

☑ Endereço IP da rede 10.24.82.0/24 obtido

☑ Comunicação com a rede funcionando

☑ Acesso à Internet validado

---

# Resultado Esperado

A máquina virtual Ubuntu Server 22.04.4 LTS estará pronta para utilização nas atividades práticas do Curso Livre de Inteligência Artificial Voltada a Redes de Computadores do SENAC São Paulo – Unidade Lapa Tito.
