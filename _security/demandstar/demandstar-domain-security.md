---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: demandstar.com
  spf: true
hosts:
- cert_expires: Sep 29 23:42:48 2026 GMT
  host: network.demandstar.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:42:48 2026 GMT
  host: www.demandstar.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Demandstar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Demandstar, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Demandstar
provider_slug: demandstar
slug: demandstar-domain-security
source_filename: demandstar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: network.demandstar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.demandstar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: demandstar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demandstar/refs/heads/main/security/demandstar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Government
- Procurement
- eProcurement
- Bids
- RFP
- Public Sector
- Supplier Network
- GovTech
- Sourcing
---
