---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ecton.io
  spf: true
hosts:
- cert_expires: Sep 28 10:42:09 2026 GMT
  host: www.ecton.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ecton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ecton, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ecton
provider_slug: ecton
slug: ecton-domain-security
source_filename: ecton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ecton.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:42:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: ecton.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecton/refs/heads/main/security/ecton-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Patient Payments
- Payments
- FinTech
- Financial Wellness
- Health Savings
- Revenue Cycle Management
- Artificial Intelligence
---
