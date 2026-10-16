---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: choco.com
  spf: true
hosts:
- cert_expires: Dec 16 13:12:06 2026 GMT
  host: choco.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Choco Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Choco Communications, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Choco Communications
provider_slug: choco-communications
slug: choco-communications-domain-security
source_filename: choco-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: choco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 13:12:06 2026 GMT\n  hsts: false\ndomains:\n- domain: choco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/choco-communications/refs/heads/main/security/choco-communications-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Food Distribution
- AI Platform
- Ecommerce
- CRM
- Sales Tools
- ERP Integration
---
