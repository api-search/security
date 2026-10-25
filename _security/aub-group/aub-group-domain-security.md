---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aubgroup.com.au
  spf: true
hosts:
- cert_expires: Nov 28 03:29:50 2026 GMT
  host: aubgroup.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aub Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AUB Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AUB Group
provider_slug: aub-group
slug: aub-group-domain-security
source_filename: aub-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aubgroup.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 03:29:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aubgroup.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aub-group/refs/heads/main/security/aub-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Insurance Broking
- Underwriting
- Financial Services
- Australia
- New Zealand
---
