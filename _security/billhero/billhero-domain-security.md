---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: billhero.com.au
  spf: true
hosts:
- cert_expires: Dec 21 10:09:35 2026 GMT
  host: billhero.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Billhero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Billhero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Billhero
provider_slug: billhero
slug: billhero-domain-security
source_filename: billhero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: billhero.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 10:09:35 2026 GMT\n  hsts: null\ndomains:\n- domain: billhero.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billhero/refs/heads/main/security/billhero-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Fintech
- Software-as-a-Service
- Australia
- Bill Management
---
