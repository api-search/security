---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: capango.com
  spf: true
hosts:
- cert_expires: Nov 25 15:35:00 2026 GMT
  host: capango.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capango Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capango, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Capango
provider_slug: capango
slug: capango-domain-security
source_filename: capango-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capango.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 15:35:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: capango.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capango/refs/heads/main/security/capango-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hiring
- Workforce
- SaaS
- ServiceEconomy
---
