---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tabcorp.com.au
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: tabcorp.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tabcorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tabcorp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tabcorp
provider_slug: tabcorp
slug: tabcorp-domain-security
source_filename: tabcorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tabcorp.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tabcorp.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabcorp/refs/heads/main/security/tabcorp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Wagering
- Betting
- Gaming
- Media
- Racing
- Australia
---
