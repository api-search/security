---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: redwoodbank.co.uk
  spf: true
hosts:
- cert_expires: Sep  6 19:17:18 2026 GMT
  host: www.redwoodbank.co.uk
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redwood Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redwood Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Redwood Bank
provider_slug: redwood-bank
slug: redwood-bank-domain-security
source_filename: redwood-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redwoodbank.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 19:17:18 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: redwoodbank.co.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redwood-bank/refs/heads/main/security/redwood-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Business Banking
- SME
- Savings
- Commercial Mortgages
- Open Banking
- PSD2
- OBIE
- United Kingdom
---
