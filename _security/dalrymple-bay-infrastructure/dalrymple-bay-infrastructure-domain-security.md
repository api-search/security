---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dbinfrastructure.com.au
  spf: true
hosts:
- cert_expires: Dec  9 19:53:33 2026 GMT
  host: dbinfrastructure.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dalrymple Bay Infrastructure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dalrymple Bay Infrastructure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dalrymple Bay Infrastructure
provider_slug: dalrymple-bay-infrastructure
slug: dalrymple-bay-infrastructure-domain-security
source_filename: dalrymple-bay-infrastructure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dbinfrastructure.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 19:53:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dbinfrastructure.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dalrymple-bay-infrastructure/refs/heads/main/security/dalrymple-bay-infrastructure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure
- Ports
- Coal Export
- Australia
- ASX Listed
- Logistics
---
