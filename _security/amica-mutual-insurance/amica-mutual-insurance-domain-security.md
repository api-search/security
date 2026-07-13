---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amica.com
  spf: true
hosts:
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: www.amica.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amica Mutual Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amica Mutual Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Amica Mutual Insurance
provider_slug: amica-mutual-insurance
slug: amica-mutual-insurance-domain-security
source_filename: amica-mutual-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amica-mutual-insurance/refs/heads/main/security/amica-mutual-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Auto Insurance
- Home Insurance
- Life Insurance
- Mutual Insurance
- Personal Insurance
- Financial Services
---
