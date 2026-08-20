---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: novo.co
  spf: true
hosts:
- cert_expires: Sep 22 11:46:48 2026 GMT
  host: novo.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Novo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Novo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Novo
provider_slug: novo
slug: novo-domain-security
source_filename: novo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: novo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:46:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: novo.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novo/refs/heads/main/security/novo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- United States
- Neobank
- Small Business Banking
- Fintech
- Open Finance
- Data Aggregation
---
