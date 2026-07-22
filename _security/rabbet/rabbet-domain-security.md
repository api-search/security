---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rabbet.com
  spf: true
hosts:
- cert_expires: Sep  2 00:10:24 2026 GMT
  host: rabbet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rabbet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rabbet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rabbet
provider_slug: rabbet
slug: rabbet-domain-security
source_filename: rabbet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rabbet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 00:10:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rabbet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rabbet/refs/heads/main/security/rabbet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Construction Finance
- Construction Lending
- Real Estate
- Draw Management
- Loan Origination
- Payments
---
