---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: b2bbank.com
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: b2bbank.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: B2B Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for B2B Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: B2B Bank
provider_slug: b2b-bank
slug: b2b-bank-domain-security
source_filename: b2b-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: b2bbank.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: b2bbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b2b-bank/refs/heads/main/security/b2b-bank-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Canada
- Schedule I Bank
- Broker Bank
- Deposits
- Mortgages
- Lending
---
