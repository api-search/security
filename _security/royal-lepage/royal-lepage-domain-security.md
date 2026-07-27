---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: royallepage.ca
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: rlpnetwork.com
  spf: false
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: www.royallepage.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.rlpnetwork.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Royal Lepage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Royal LePage, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Royal LePage
provider_slug: royal-lepage
slug: royal-lepage-domain-security
source_filename: royal-lepage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.royallepage.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\n- host: www.rlpnetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: royallepage.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rlpnetwork.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/royal-lepage/refs/heads/main/security/royal-lepage-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Canada
- Property Listings
- MLS
- Brokerage
- IDX
- VOW
- Residential Real Estate
- Franchise
- PropTech
---
