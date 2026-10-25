---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nrw.com.au
  spf: true
hosts:
- cert_expires: Dec 21 07:04:40 2026 GMT
  host: nrw.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nrw Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NRW Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NRW Holdings
provider_slug: nrw-holdings
slug: nrw-holdings-domain-security
source_filename: nrw-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nrw.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 07:04:40 2026 GMT\n  hsts: false\ndomains:\n- domain: nrw.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nrw-holdings/refs/heads/main/security/nrw-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Construction
- Mining Services
- Civil Engineering
- Engineering
- Maintenance
- Australia
- ASX Listed
---
