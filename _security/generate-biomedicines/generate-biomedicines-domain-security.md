---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: generatebiomedicines.com
  spf: true
hosts:
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: generatebiomedicines.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Generate Biomedicines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Generate Biomedicines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Generate Biomedicines
provider_slug: generate-biomedicines
slug: generate-biomedicines-domain-security
source_filename: generate-biomedicines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: generatebiomedicines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: generatebiomedicines.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/generate-biomedicines/refs/heads/main/security/generate-biomedicines-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Generative Biology
- Protein Design
- De Novo Design
- Diffusion Models
- Antibodies
- Drug Discovery
- Therapeutics
- Machine Learning
- Biotechnology
- Chroma
- Foundation Models
- Equivariant Neural Networks
- Flagship Pioneering
---
