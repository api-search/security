---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ororagroup.com
  spf: true
hosts:
- cert_expires: Apr 18 23:59:59 2027 GMT
  host: ororagroup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Orora
provider_slug: orora
slug: orora-domain-security
source_filename: orora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ororagroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ororagroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orora/refs/heads/main/security/orora-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Packaging
- Manufacturing
- Glass
- Aluminium Cans
- Beverage
- Sustainability
- Australia
- ASX Listed
---
