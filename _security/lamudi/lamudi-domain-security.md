---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lamudi.com.ph
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lamudi.co.id
  spf: true
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: www.lamudi.com.ph
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: www.lamudi.co.id
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.lamudi.com.mx
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lamudi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lamudi, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lamudi
provider_slug: lamudi
slug: lamudi-domain-security
source_filename: lamudi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lamudi.com.ph\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\n- host: www.lamudi.co.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\n- host: www.lamudi.com.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lamudi.com.ph\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: lamudi.co.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lamudi/refs/heads/main/security/lamudi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- Real Estate
- Property
- Classifieds
- Emerging Markets
- Philippines
- Indonesia
- Mexico
- Listings
---
