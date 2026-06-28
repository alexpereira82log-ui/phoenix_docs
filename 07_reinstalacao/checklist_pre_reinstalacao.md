# Checklist Pré-Reinstalação

## Objetivo

Garantir que todas as informações críticas do ambiente atual estejam preservadas antes da reinstalação do sistema operacional.

A reinstalação somente deverá ser iniciada após todos os itens deste documento estarem validados.

---

# 1. Controle de Versão

| Item                                      | Como verificar               | Resultado esperado                          | Status |
| ----------------------------------------- | ---------------------------- | ------------------------------------------- | ------ |
| Todos os repositórios sincronizados       | `git status` em cada projeto | Working tree clean ou alterações conhecidas | ☐      |
| Alterações importantes enviadas ao GitHub | `git push`                   | Repositório remoto atualizado               | ☐      |

---

# 2. Projeto Phoenix

| Item                             | Como verificar         | Resultado esperado             | Status |
| -------------------------------- | ---------------------- | ------------------------------ | ------ |
| Inventário atualizado            | Revisar `phoenix_docs` | Documentação completa          | ☐      |
| Plano de reinstalação atualizado | Revisar documentação   | Versão mais recente disponível | ☐      |

---

# 3. Configurações do Usuário

| Item                           | Como verificar               | Resultado esperado       | Status |
| ------------------------------ | ---------------------------- | ------------------------ | ------ |
| Backup do dconf                | Verificar `dconf_backup.ini` | Arquivo presente         | ☐      |
| Chaves SSH preservadas         | Verificar `~/.ssh`           | Chaves disponíveis       | ☐      |
| Configuração do Git registrada | Verificar `~/.gitconfig`     | Configuração documentada | ☐      |

---

# 4. Ambiente de Desenvolvimento

| Item                                | Como verificar               | Resultado esperado      | Status |
| ----------------------------------- | ---------------------------- | ----------------------- | ------ |
| Requirements dos projetos revisados | Verificar `requirements.txt` | Arquivos presentes      | ☐      |
| Projetos sincronizados              | Revisar GitHub               | Última versão publicada | ☐      |

---

# 5. Obsidian

| Item                      | Como verificar            | Resultado esperado       | Status |
| ------------------------- | ------------------------- | ------------------------ | ------ |
| Vault sincronizado        | Verificar GitHub          | Últimos commits enviados | ☐      |
| Configurações preservadas | Revisar pasta `.obsidian` | Arquivos presentes       | ☐      |

---

# 6. Backup

| Item                                        | Como verificar          | Resultado esperado  | Status |
| ------------------------------------------- | ----------------------- | ------------------- | ------ |
| Snapshot recente disponível                 | `sudo timeshift --list` | Snapshot atualizado | ☐      |
| Backup externo conferido (quando aplicável) | Verificação manual      | Backup íntegro      | ☐      |

---

# Critério para início da reinstalação

A reinstalação somente poderá ser iniciada quando:

* todos os itens críticos estiverem concluídos;
* nenhum item permanecer pendente sem justificativa;
* existir pelo menos um snapshot recente e validado;
* os repositórios estiverem sincronizados com o GitHub.

---

# Observações

Este checklist deverá ser executado imediatamente antes da reinstalação do sistema.

Quaisquer divergências identificadas deverão ser resolvidas antes de prosseguir com o processo.

