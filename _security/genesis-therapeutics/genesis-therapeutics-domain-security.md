---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: genesis.ml
  spf: true
hosts:
- cert_expires: Oct  3 03:45:29 2026 GMT
  host: genesis.ml
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genesis Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genesis Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Genesis Therapeutics
provider_slug: genesis-therapeutics
slug: genesis-therapeutics-domain-security
source_filename: genesis-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genesis.ml\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:45:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: genesis.ml\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genesis-therapeutics/refs/heads/main/security/genesis-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Drug Discovery
- Biotechnology
- Life Sciences
- Pharmaceuticals
- Molecular AI
---
