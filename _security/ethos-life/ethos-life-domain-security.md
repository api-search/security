---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ethos.com
  spf: true
hosts:
- cert_expires: Oct  2 15:10:55 2026 GMT
  host: www.ethos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ethos Life Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ethos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ethos
provider_slug: ethos-life
slug: ethos-life-domain-security
source_filename: ethos-life-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ethos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:10:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ethos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethos-life/refs/heads/main/security/ethos-life-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Life Insurance
- Term Life Insurance
- Whole Life Insurance
- Indexed Universal Life
- Insurtech
- Digital Insurance
- No Medical Exam
- Underwriting
- Quotes
- Policies
- Embedded Insurance
- Partnership API
- Financial Services
---
