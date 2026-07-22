---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nmrk.com
  spf: true
hosts:
- cert_expires: Sep 10 11:47:49 2026 GMT
  host: www.nmrk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newmark Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newmark Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Newmark Group
provider_slug: newmark-group
slug: newmark-group-domain-security
source_filename: newmark-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nmrk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 11:47:49 2026 GMT\n  hsts: null\ndomains:\n- domain: nmrk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newmark-group/refs/heads/main/security/newmark-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Commercial Real Estate
- Capital Markets
- Leasing
- Valuation
- Property Management
- Global Corporate Services
- Industrial
- Multifamily
- Public Company
---
