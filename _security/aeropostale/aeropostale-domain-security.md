---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aeropostale.com
  spf: true
hosts:
- cert_expires: Aug  6 16:23:54 2026 GMT
  host: www.aeropostale.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aeropostale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aéropostale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aéropostale
provider_slug: aeropostale
slug: aeropostale-domain-security
source_filename: aeropostale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aeropostale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  6 16:23:54 2026 GMT\n  hsts: null\ndomains:\n- domain: aeropostale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeropostale/refs/heads/main/security/aeropostale-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Retail
- Fashion
- Teen Apparel
---
