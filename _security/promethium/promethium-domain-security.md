---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: promethium.ai
  spf: true
hosts:
- cert_expires: Oct 14 03:29:18 2026 GMT
  host: promethium.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 02:14:49 2026 GMT
  host: docs.promethium.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: api.prod.promethium.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Promethium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Promethium, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Promethium
provider_slug: promethium
slug: promethium-domain-security
source_filename: promethium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: promethium.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 03:29:18 2026 GMT\n  hsts: false\n- host: docs.promethium.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 02:14:49 2026 GMT\n  hsts: false\n- host: api.prod.promethium.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: promethium.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/promethium/refs/heads/main/security/promethium-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data Fabric
- Agentic Analytics
- Semantic Layer
- Enterprise Data
- Model Context Protocol
- Federated Query
- Data Governance
---
