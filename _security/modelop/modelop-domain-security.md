---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modelop.com
  spf: true
- caa:
  - 0 issuewild "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atlassian.net
  spf: true
hosts:
- cert_expires: Oct 14 14:58:52 2026 GMT
  host: www.modelop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: modelopdocs.atlassian.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modelop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ModelOp, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ModelOp
provider_slug: modelop
slug: modelop-domain-security
source_filename: modelop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.modelop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 14:58:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: modelopdocs.atlassian.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: modelop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: atlassian.net\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nhost_ownership_note: >-\n  modelopdocs.atlassian.net is Atlassian-owned Confluence Cloud,\
  \ not a ModelOp-controlled host —\n  it appears here only because it is the humanURL for the ModelOp Center REST API entry. Its TLS,\n  HSTS, CAA and DMARC posture (including dmarc_policy reject) belongs to Atlassian and must not be\n  read as ModelOp's own. The provider-controlled row is modelop.com / www.modelop.com:\n  TLS 1.3, HSTS max-age 31536000, SPF present, DMARC present with policy `none` (monitor only),\n  no DNSSEC and no CAA records.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modelop/refs/heads/main/security/modelop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Governance
- Model Risk Management
- Machine-Learning
- MLOps
- ModelOps
- AI Lifecycle Automation
- Enterprise Software
- Compliance
- Model Monitoring
- Governance Risk and Compliance
- Artificial Intelligence
---
