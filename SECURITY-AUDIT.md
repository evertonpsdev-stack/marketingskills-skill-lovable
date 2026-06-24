# Security audit — coreyhaines31/marketingskills

**Risco:** CLEAN (após mitigação)
**Achados originais:** 1 · todos neutralizados

A skill foi sanitizada client-side: snippets perigosos (curl|sh, eval, credenciais, domínios de exfiltração, hooks de lifecycle do npm, etc.) foram removidos ou desativados em todos os arquivos do pacote (`REFERENCES.md`, `_package.json`, demais textos).

## Achados originalmente detectados

### [CRITICAL] Env exfiltration pattern — `tools/clis/zoominfo.js`

Lê variáveis de ambiente e envia por HTTP — padrão clássico de roubo de credenciais.

_Trecho neutralizado._
