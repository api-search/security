---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: compound.xyz
  spf: true
hosts:
- cert_expires: Dec 29 17:52:20 2026 GMT
  host: www.compound.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Compound Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Compound Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Compound Finance
provider_slug: compound-finance
slug: compound-finance-domain-security
source_filename: compound-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.compound.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 17:52:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: compound.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/compound-finance/refs/heads/main/security/compound-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Finance
- Lending
- Cryptocurrency
- Blockchain
---
