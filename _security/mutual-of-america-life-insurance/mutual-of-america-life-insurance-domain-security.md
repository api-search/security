---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mutualofamerica.com
  spf: true
hosts:
- cert_expires: Nov 10 09:18:05 2026 GMT
  host: www.mutualofamerica.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mutual Of America Life Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mutual of America Life Insurance Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mutual of America Life Insurance Company
provider_slug: mutual-of-america-life-insurance
slug: mutual-of-america-life-insurance-domain-security
source_filename: mutual-of-america-life-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mutualofamerica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 09:18:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mutualofamerica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mutual-of-america-life-insurance/refs/heads/main/security/mutual-of-america-life-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Life Insurance
- Retirement
- Financial Services
- Pensions
- Annuities
- Wealth Management
- Identity
---
