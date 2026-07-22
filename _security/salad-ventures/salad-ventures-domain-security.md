---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: salad.ventures
  spf: true
hosts:
- cert_expires: Oct 18 07:30:05 2026 GMT
  host: salad.ventures
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salad Ventures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salad Ventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Salad Ventures
provider_slug: salad-ventures
slug: salad-ventures-domain-security
source_filename: salad-ventures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: salad.ventures\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 07:30:05 2026 GMT\n  hsts: null\ndomains:\n- domain: salad.ventures\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salad-ventures/refs/heads/main/security/salad-ventures-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Venture Capital
- Investment
- Blockchain
- Web3 Gaming
- Digital Assets
---
