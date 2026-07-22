---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plans.app
  spf: true
hosts:
- cert_expires: Oct 16 20:40:34 2026 GMT
  host: plans.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plans Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plans, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plans
provider_slug: plans
slug: plans-domain-security
source_filename: plans-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plans.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 20:40:34 2026 GMT\n  hsts: false\ndomains:\n- domain: plans.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plans/refs/heads/main/security/plans-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Climate
- Energy
- Decarbonization
- Built World
- Home Retrofit
- Construction Tech
- Sustainability
---
