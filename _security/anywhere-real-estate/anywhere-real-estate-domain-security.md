---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anywhere.re
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: realogy.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: anywhere.re
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 22:32:53 2026 GMT
  host: developers.anywhere.re
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: api.realogy.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Anywhere Real Estate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anywhere Real Estate, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Anywhere Real Estate
provider_slug: anywhere-real-estate
slug: anywhere-real-estate-domain-security
source_filename: anywhere-real-estate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anywhere.re\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.anywhere.re\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:32:53 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api.realogy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: anywhere.re\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: realogy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anywhere-real-estate/refs/heads/main/security/anywhere-real-estate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- United States
- Property Listings
- MLS
- RESO
- Brokerage
- Franchising
- PropTech
- Title
- Escrow
- Relocation
- Leads
- Transactions
---
