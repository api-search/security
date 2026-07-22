---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dcg.co
  spf: true
hosts:
- cert_expires: Oct  7 09:12:48 2026 GMT
  host: dcg.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digital Currency Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digital Currency Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Digital Currency Group
provider_slug: digital-currency-group
slug: digital-currency-group-domain-security
source_filename: digital-currency-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dcg.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:12:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dcg.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digital-currency-group/refs/heads/main/security/digital-currency-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Cryptocurrency
- Blockchain
- Digital Assets
- Venture Capital
- Investment
---
