---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paytient.com
  spf: true
hosts:
- cert_expires: Sep 28 10:44:17 2026 GMT
  host: paytient.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paytient Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paytient, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paytient
provider_slug: paytient
slug: paytient-domain-security
source_filename: paytient-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paytient.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:44:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: paytient.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paytient/refs/heads/main/security/paytient-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Healthcare
- Payments
- Fintech
- Health Benefits
- Lending
---
