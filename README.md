# BioSaude-Nacional
Analise de Segurança, gestão de riscos, compliance e aplicação de LGDP da Empresa Ficticia BioSaude

BioSaúde Nacional — BSN
Análise de Segurança, Gestão de Riscos, Compliance e Aplicação da LGPD
1. Identificação da Empresa

**Nome:** BioSaúde Nacional — BSN

**Natureza:** Empresa pública estadual fictícia

**Setor:** Saúde, biotecnologia e produção de insumos estratégicos

1.1 Atuação

A BioSaúde Nacional atua nas seguintes áreas:

- Produção e distribuição de vacinas;
- Produção e distribuição de insumos biológicos;
- Produção de produtos bioquímicos;
- Produção e distribuição de medicamentos e fármacos;
- Armazenamento de materiais sensíveis;
- Pesquisa e desenvolvimento;
- Distribuição de produtos para hospitais e unidades de saúde.

**2. Objetivo da Avaliação**

Realizar uma avaliação fictícia de Governança, Riscos e Compliance (GRC), com foco na segurança da informação e na infraestrutura tecnológica da empresa BioSaúde Nacional.

A avaliação utiliza como principais referências:

ISO/IEC 27001:2022 — Sistema de Gestão de Segurança da Informação (SGSI);

ISO/IEC 27005:2022 — Gestão de riscos de segurança da informação;

ISO/IEC 27002:2022 — Controles de segurança da informação;

NIST Cybersecurity Framework (CSF) 2.0;

CIS Controls v8.1;

Lei Geral de Proteção de Dados Pessoais (LGPD — Lei nº 13.709/2018).

**3. Panorama da Infraestrutura Atual**

O panorama da infraestrutura tecnológica atual da BioSaúde Nacional está representado no diagrama de rede:

Arquivo de referência: diagram-network.png

Observação: o diagrama de rede deve ser disponibilizado junto a este documento para complementar a análise da infraestrutura.

**4. Achados de Segurança**
**FDG-001 — Ausência de MFA para Acesso Remoto Administrativo**
4.1 Identificação
Campo	Informação
ID	FDG-001
Ativo associado	VPN Corporativa
Risco	Alto
Categoria	Controle de acesso / Autenticação
Status	Não implementado
4.2 Evidência Simulada

A VPN corporativa permite autenticação somente por meio de usuário e senha.

Não foi identificada a implementação de MFA (Multi-Factor Authentication) para contas administrativas e acessos remotos privilegiados.

4.3 Impactos Potenciais

A ausência de autenticação multifator pode aumentar significativamente o risco de comprometimento da infraestrutura corporativa.

Entre os possíveis impactos estão:

Comprometimento de contas administrativas;
Acesso indevido à rede corporativa;
Movimento lateral dentro da infraestrutura;
Escalonamento de privilégios;
Indisponibilidade de sistemas e serviços;
Possível exposição de dados sensíveis;
Comprometimento de sistemas críticos;
Aumento do impacto de ataques decorrentes de credenciais comprometidas.
4.4 Recomendação

Implementar MFA (Multi-Factor Authentication) obrigatoriamente para:

Acessos remotos à rede corporativa;
Contas administrativas;
Contas privilegiadas;
Acesso à VPN;
Sistemas críticos;
Serviços de infraestrutura que permitam autenticação remota.

Sempre que tecnicamente viável, recomenda-se priorizar mecanismos de autenticação resistentes a phishing para contas privilegiadas e administrativas.

4.5 Referências e Frameworks Relacionados

O achado possui relação com os seguintes referenciais:

ISO/IEC 27001:2022;
ISO/IEC 27002:2022;
ISO/IEC 27005:2022;
NIST Cybersecurity Framework 2.0;
CIS Controls v8.1;
LGPD, especialmente no contexto de adoção de medidas técnicas e administrativas destinadas à proteção de dados pessoais.
5. Resumo do Achado
ID	Achado	Ativo	Risco	Recomendação
FDG-001	Ausência de MFA para acesso remoto administrativo	VPN Corporativa	Alto	Implementar MFA para acesso remoto e contas privilegiadas


