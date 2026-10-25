---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vicinity.com.au
  spf: true
hosts:
- cert_expires: Dec 23 12:31:36 2026 GMT
  host: vicinity.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vicinity Centres Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vicinity Centres, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vicinity Centres
provider_slug: vicinity-centres
slug: vicinity-centres-domain-security
source_filename: vicinity-centres-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vicinity.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 12:31:36 2026 GMT\n  hsts: null\ndomains:\n- domain: vicinity.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vicinity-centres/refs/heads/main/security/vicinity-centres-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- Real Estate
- Shopping Centres
- Property Management
- Australia
- Leasing
---
