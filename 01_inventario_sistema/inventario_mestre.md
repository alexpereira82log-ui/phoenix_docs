# Inventário Mestre do Sistema

## Projeto

**Projeto Phoenix**
Reconstrução completa do ambiente Linux.

---

# Sistema Operacional

* Distribuição: Pop!_OS 22.04 LTS
* Base: Ubuntu Jammy
* ID: pop
* Arquitetura: x86_64

---

# Kernel

* Versão: 7.0.11-76070011-generic

---

# Hardware

## Fabricante

Lenovo

## Modelo

IdeaPad Slim 3 15ARP10

---

# Processador

* AMD Ryzen 7 7735HS with Radeon Graphics

* 8 núcleos físicos

* 16 threads

* Frequência máxima aproximada: 4.83 GHz

* Virtualização AMD-V habilitada

---

# Memória RAM

* Total: 19 GiB

---

# Disco Principal

* Tipo: NVMe SSD

Dispositivo:

```
/dev/nvme0n1
```

---

# Partições atuais

## p1

EFI Windows

FAT32

---

## p2

Microsoft Reserved (MSR)

---

## p3

Windows

BitLocker

Aproximadamente 220 GiB

---

## Espaço não alocado

Aproximadamente 157 GiB

Reservado para futura reinstalação do Pop!_OS.

---

## p5

Swap Linux

2 GiB

---

## p6

EFI do Pop!_OS

FAT32

UUID:

```
1D66-C3BB
```

---

## p7

Sistema principal Linux

Btrfs

UUID:

```
576fee26-8a3a-4247-9263-8199dbb10a47
```

Tamanho aproximado:

95 GiB

Espaço utilizado:

75 GiB

Espaço livre:

19 GiB

---

## p4

Recovery do Windows

NTFS

---

# Situação atual do Projeto Phoenix

* Reinstalação planejada.
* Expansão direta cancelada por opção estratégica.
* Objetivo: reinstalar o Pop!_OS utilizando aproximadamente 250 GiB.
* Preservar integralmente o Windows.
* Reconstruir o ambiente de forma praticamente idêntica ao original.

---

# Filosofia do projeto

Todo o ambiente deverá ser reconstruível apenas utilizando a documentação presente no repositório `phoenix_docs`.
