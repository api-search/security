---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fifteenth.com
  spf: true
hosts:
- cert_expires: Sep 22 15:41:51 2026 GMT
  host: www.fifteenth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fifteenth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fifteenth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fifteenth
provider_slug: fifteenth
slug: fifteenth-domain-security
source_filename: fifteenth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fifteenth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:41:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fifteenth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fifteenth/refs/heads/main/security/fifteenth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Taxes
- Tax Preparation
- Tax Planning
- Personal Finance
- Equity Compensation
- Accounting
- Artificial Intelligence
---
