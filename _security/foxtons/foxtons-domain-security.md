---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: foxtons.co.uk
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: foxtonsgroup.co.uk
  spf: true
hosts:
- cert_expires: Oct  9 23:41:00 2026 GMT
  host: www.foxtons.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 05:53:51 2026 GMT
  host: www.foxtonsgroup.co.uk
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Foxtons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foxtons, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Foxtons
provider_slug: foxtons
slug: foxtons-domain-security
source_filename: foxtons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foxtons.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:41:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.foxtonsgroup.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 05:53:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: foxtons.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: foxtonsgroup.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foxtons/refs/heads/main/security/foxtons-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- United Kingdom
- Property Listings
- Rentals
- Lettings
- Property Management
- Estate Agency
- Mortgage
- PropTech
- London
---
