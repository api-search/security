---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stayukio.com
  spf: true
hosts:
- cert_expires: Sep 26 04:04:08 2026 GMT
  host: www.stayukio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ukio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ukio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ukio
provider_slug: ukio
slug: ukio-domain-security
source_filename: ukio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stayukio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 04:04:08 2026 GMT\n  hsts: null\ndomains:\n- domain: stayukio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ukio/refs/heads/main/security/ukio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Real Estate
- PropTech
- Housing
- Rentals
- Corporate Housing
- Travel
---
