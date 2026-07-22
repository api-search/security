---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arbilex.co
  spf: true
hosts:
- cert_expires: Oct  4 01:06:10 2026 GMT
  host: arbilex.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arbilex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ArbiLex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ArbiLex
provider_slug: arbilex
slug: arbilex-domain-security
source_filename: arbilex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arbilex.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:06:10 2026 GMT\n  hsts: null\ndomains:\n- domain: arbilex.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arbilex/refs/heads/main/security/arbilex-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Legal
- LegalTech
- Litigation Finance
- Arbitration
- Legal Analytics
- Artificial Intelligence
- Predictive Analytics
- Fintech
---
