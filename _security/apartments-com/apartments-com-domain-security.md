---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "godaddy.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apartments.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.apartments.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apartments Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apartments.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apartments.com
provider_slug: apartments-com
slug: apartments-com-domain-security
source_filename: apartments-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apartments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: apartments.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apartments-com/refs/heads/main/security/apartments-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real-Estate
- United States
- Rentals
- Property Listings
- Multifamily
- Internet Listing Service
- Listings Syndication
- Property Management
- MLS
- PropTech
- CoStar Group
---
