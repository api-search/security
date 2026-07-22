---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: miuros.com
  spf: true
hosts:
- cert_expires: Sep 24 04:05:36 2026 GMT
  host: miuros.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Miuros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Miuros, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Miuros
provider_slug: miuros
slug: miuros-domain-security
source_filename: miuros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: miuros.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:05:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: miuros.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miuros/refs/heads/main/security/miuros-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Service
- Customer Support
- Analytics
- Quality Assurance
- Artificial Intelligence
- SaaS
- Techstars
---
