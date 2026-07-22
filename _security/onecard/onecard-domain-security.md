---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getonecard.app
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: www.getonecard.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onecard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onecard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Onecard
provider_slug: onecard
slug: onecard-domain-security
source_filename: onecard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getonecard.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getonecard.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onecard/refs/heads/main/security/onecard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Credit
- Fintech
- Credit Card
- Payments
- Banking
- India
- Consumer Finance
---
