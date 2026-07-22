---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: imotorbike.com
  spf: true
hosts:
- cert_expires: Sep 29 02:56:56 2026 GMT
  host: imotorbike.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imotorbike Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iMotorbike, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iMotorbike
provider_slug: imotorbike
slug: imotorbike-domain-security
source_filename: imotorbike-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imotorbike.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:56:56 2026 GMT\n  hsts: false\ndomains:\n- domain: imotorbike.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imotorbike/refs/heads/main/security/imotorbike-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- Motorcycles
- Automotive
- E-Commerce
- Southeast Asia
- Malaysia
- Vietnam
- Used Vehicles
- Inspection
---
