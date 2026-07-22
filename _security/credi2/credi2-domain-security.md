---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: credi2.com
  spf: true
hosts:
- cert_expires: Sep  7 21:11:27 2026 GMT
  host: www.credi2.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Credi2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credi2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Credi2
provider_slug: credi2
slug: credi2-domain-security
source_filename: credi2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.credi2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:11:27 2026 GMT\n  hsts: false\ndomains:\n- domain: credi2.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credi2/refs/heads/main/security/credi2-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Embedded Finance
- Lending
- Buy Now Pay Later
- BNPL
- Installments
- Fintech
- Banking
- Card Issuing
- Credit
---
