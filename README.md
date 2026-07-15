# security-agent-skills-arsenal

Indice de forks `maux339-cpu` — pentest, malware analysis (pesquisa), DeFi/SC.

**Uso autorizado apenas** (audit, bounty, CTF, lab). Nao e kit de ataque a mainnet.

---

## Mapa: tipo de exploit → skill / ferramenta

Base: o que ja esta forkado no account. Ordem sugerida = **detectar → entender padrao → reproduzir em lab → reportar**.

### 1) Reentrancy (classic / cross-function / read-only / ERC777)

| Fase | Onde ir |
|------|---------|
| Padrao + lista real | [reentrancy-attacks](https://github.com/maux339-cpu/reentrancy-attacks) |
| Labs | [DeFiHackLabs](https://github.com/maux339-cpu/DeFiHackLabs), [damn-vulnerable-defi](https://github.com/maux339-cpu/damn-vulnerable-defi), [ethernaut](https://github.com/maux339-cpu/ethernaut) |
| Static | [slither](https://github.com/maux339-cpu/slither) (`reentrancy-*`), [aderyn](https://github.com/maux339-cpu/aderyn) |
| Skills AI audit | [trailofbits-skills](https://github.com/maux339-cpu/trailofbits-skills), [pashov-skills](https://github.com/maux339-cpu/pashov-skills), [solskill](https://github.com/maux339-cpu/solskill) |
| Guia | [building-secure-contracts](https://github.com/maux339-cpu/building-secure-contracts) |
| PoC report | [forge-poc-templates](https://github.com/maux339-cpu/forge-poc-templates) + [foundry](https://github.com/maux339-cpu/foundry) |

### 2) Flash loan / price oracle manipulation

| Fase | Onde ir |
|------|---------|
| Casos reais | [DeFiHackLabs](https://github.com/maux339-cpu/DeFiHackLabs) (buscar flashloan/oracle) |
| Labs | [damn-vulnerable-defi](https://github.com/maux339-cpu/damn-vulnerable-defi), [DeFiVulnLabs](https://github.com/maux339-cpu/DeFiVulnLabs) |
| Skills | [pashov-skills](https://github.com/maux339-cpu/pashov-skills), [sc-auditor](https://github.com/maux339-cpu/sc-auditor), [quillshield_skills](https://github.com/maux339-cpu/quillshield_skills) |
| Fuzz econ | [medusa](https://github.com/maux339-cpu/medusa), [echidna](https://github.com/maux339-cpu/echidna) |
| Intel | [Knowledge-Base](https://github.com/maux339-cpu/Knowledge-Base) (SlowMist), [Web3-Security-Library](https://github.com/maux339-cpu/Web3-Security-Library) |

### 3) Access control / privilege / ownership / proxy admin

| Fase | Onde ir |
|------|---------|
| Static | [slither](https://github.com/maux339-cpu/slither), [mythril](https://github.com/maux339-cpu/mythril), [aderyn](https://github.com/maux339-cpu/aderyn) |
| Skills | [trailofbits-skills](https://github.com/maux339-cpu/trailofbits-skills), [solskill](https://github.com/maux339-cpu/solskill), [scv-scan](https://github.com/maux339-cpu/scv-scan) |
| Labs | [ethernaut](https://github.com/maux339-cpu/ethernaut), [DeFiVulnLabs](https://github.com/maux339-cpu/DeFiVulnLabs) |
| Compêndio | [Solidity-Security-Compendium](https://github.com/maux339-cpu/Solidity-Security-Compendium) |

### 4) Logic bugs / business logic / invariants

| Fase | Onde ir |
|------|---------|
| Skills auditor | [pashov-skills](https://github.com/maux339-cpu/pashov-skills), [sc-auditor](https://github.com/maux339-cpu/sc-auditor) |
| Fuzz + formal | [echidna](https://github.com/maux339-cpu/echidna), [medusa](https://github.com/maux339-cpu/medusa), [halmos](https://github.com/maux339-cpu/halmos), [kontrol](https://github.com/maux339-cpu/kontrol), [hevm](https://github.com/maux339-cpu/hevm), Certora [Tutorials](https://github.com/maux339-cpu/Tutorials) |
| Casos | [DeFiHackLabs](https://github.com/maux339-cpu/DeFiHackLabs), [solodit_content](https://github.com/maux339-cpu/solodit_content) |
| Bench AI | [evmbench](https://github.com/maux339-cpu/evmbench) |

### 5) Rug / honeypot / hidden mint / backdoor owner

| Fase | Onde ir |
|------|---------|
| Skills + L2 | [kali-claw](https://github.com/maux339-cpu/kali-claw) (`blockchain-web3`, `blockchain-l2-attack`) |
| Skills audit | [quillshield_skills](https://github.com/maux339-cpu/quillshield_skills), [scv-scan](https://github.com/maux339-cpu/scv-scan) |
| Static | [slither](https://github.com/maux339-cpu/slither), [aderyn](https://github.com/maux339-cpu/aderyn) |
| Self-guard | [Blockchain-dark-forest-selfguard-handbook](https://github.com/maux339-cpu/Blockchain-dark-forest-selfguard-handbook) |
| Compêndio | [Solidity-Security-Compendium](https://github.com/maux339-cpu/Solidity-Security-Compendium) |

### 6) Bridge / L2 / sequencer / cross-chain

| Fase | Onde ir |
|------|---------|
| Skills | [kali-claw](https://github.com/maux339-cpu/kali-claw) L2 skill |
| Labs/casos | [DeFiHackLabs](https://github.com/maux339-cpu/DeFiHackLabs), contests [code-423n4](https://github.com/maux339-cpu/2026-04-layerzero) |
| Intel | [Knowledge-Base](https://github.com/maux339-cpu/Knowledge-Base), [audit-reports](https://github.com/maux339-cpu/audit-reports) (BlockSec) |

### 7) Flashbots / MEV-style / sandwich (estudo)

| Fase | Onde ir |
|------|---------|
| Casos DeFi | [DeFiHackLabs](https://github.com/maux339-cpu/DeFiHackLabs) |
| Tooling tx | [Phalcon](https://github.com/maux339-cpu/Phalcon), [web3-companion](https://github.com/maux339-cpu/web3-companion) |
| Skills | [pashov-skills](https://github.com/maux339-cpu/pashov-skills) (review de design) |

### 8) Plataforma CEX / exchange web (nao SC)

| Fase | Onde ir |
|------|---------|
| Web ofensivo (auth) | [Claude-Red](https://github.com/maux339-cpu/Claude-Red), [Claude-BugHunter](https://github.com/maux339-cpu/Claude-BugHunter), [claude-bug-bounty](https://github.com/maux339-cpu/claude-bug-bounty) |
| OSINT DeFi | [arsenal-osint-defi-2026](https://github.com/maux339-cpu/arsenal-osint-defi-2026) |
| Report | [offensive-reporting] patterns via BugHunter |

**So com autorizacao escrita / programa de bounty.**

### 9) Report / triage / PoC

| Item | Repo |
|------|------|
| Template PoC Foundry | [forge-poc-templates](https://github.com/maux339-cpu/forge-poc-templates) |
| Findings database | [solodit_content](https://github.com/maux339-cpu/solodit_content), [4naly3er](https://github.com/maux339-cpu/4naly3er) |
| Skills review | [trailofbits-skills](https://github.com/maux339-cpu/trailofbits-skills), [claude-code-security-review](https://github.com/maux339-cpu/claude-code-security-review) |

---

## Fluxo rapido (1 alvo SC)

1. **Recon codigo** → solskill / pashov-skills / trailofbits-skills  
2. **Static** → slither + aderyn (+ mythril se quiser)  
3. **Padroes** → Solidity-Security-Compendium + building-secure-contracts  
4. **Parecidos** → DeFiHackLabs / solodit  
5. **Invariantes** → echidna/medusa ou halmos/kontrol  
6. **PoC** → foundry + forge-poc-templates  
7. **Report** → template Immunefi/C4  

---

## Catalogo de forks (resumo)

### Skills SC/AI
pashov-skills · trailofbits-skills · solskill · scv-scan · quillshield_skills · sc-auditor · claude-code-security-review · kali-claw

### Labs
DeFiHackLabs · DeFiVulnLabs · damn-vulnerable-defi · ethernaut · reentrancy-attacks

### Tools
slither · echidna · medusa · mythril · aderyn · foundry · hevm · kontrol ·halmos · forge-poc-templates · 4naly3er

### Intel
Knowledge-Base · Web3-Security-Library · Blockchain-dark-forest-selfguard-handbook · solodit_content · audit-reports

### Web / red team (plataformas)
Claude-Red · Claude-BugHunter · claude-bug-bounty · red-run · offensive-claude · ctf-skills

### Malware analysis (pesquisa)
capa · CAPEv2 · volatility3 · signature-base · analyst-ai-pack

---

Atualizado 2026-07-15 — mapa exploit×skill executado via API (sem clone local).