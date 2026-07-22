---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apartmentlist.com
  spf: true
hosts:
- cert_expires: Dec 22 18:10:14 2026 GMT
  host: www.apartmentlist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apartment List Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apartment List, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apartment List
provider_slug: apartment-list
slug: apartment-list-domain-security
source_filename: apartment-list-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apartmentlist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 18:10:14 2026 GMT\n  hsts: false\ndomains:\n- domain: apartmentlist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apartment-list/refs/heads/main/security/apartment-list-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Rentals
- Real Estate
- Housing
- Apartments
- Marketplace
- PropTech
- Consumer
---
