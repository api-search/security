---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hebbia.com
  spf: true
hosts:
- cert_expires: Aug 15 16:47:30 2026 GMT
  host: www.hebbia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hebbia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hebbia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hebbia
provider_slug: hebbia
slug: hebbia-domain-security
source_filename: hebbia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hebbia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 16:47:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hebbia.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hebbia/refs/heads/main/security/hebbia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Document AI
- Due Diligence
- Enterprise Search
- Financial Services
- Generative AI
- Investment Research
- Knowledge
- Matrix
- RAG
- Research
- Unstructured Data
---
