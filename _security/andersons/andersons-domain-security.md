---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: andersonsinc.com
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: www.andersonsinc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Andersons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Andersons, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: The Andersons
provider_slug: andersons
slug: andersons-domain-security
source_filename: andersons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.andersonsinc.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: andersonsinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andersons/refs/heads/main/security/andersons-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Agribusiness
- Agriculture
- Grain
- Commodity Merchandising
- Plant Nutrients
- Fertilizer
- Renewables
- Ethanol
- Food and Feed Ingredients
- Turf and Specialty Products
- Rail Leasing
- Supply Chain
---
