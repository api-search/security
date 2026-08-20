---
api_specs:
- filename: re-max-canada-blog-wp-json-index.json
  format: json
  label: RE/MAX Canada Blog WordPress REST API
  slug: re-max-canada-blog-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/re-max-canada/refs/heads/main/openapi/re-max-canada-blog-wp-json-index.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: remax.ca
  spf: true
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: www.remax.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 13:51:50 2026 GMT
  host: blog.remax.ca
  hsts: false
  https: true
  note: The API host (baseURL https://blog.remax.ca/wp-json). Probed by hand this round because the mechanical sweep did not include it. WordPress VIP nginx; no Strict-Transport-Security header returned.
  tls_version: TLSv1.3
- cert_expires: Sep 30 15:07:01 2026 GMT
  host: agentbrokerhub.remax.ca
  hsts: false
  https: true
  note: Real WordPress VIP host discovered this round (CNAME remax-promotions.go-vip.net), distinct from the remax.ca DNS wildcard.
  tls_version: TLSv1.3
- cert_expires: Sep  1 22:54:22 2026 GMT
  host: franchise.remax.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 00:52:21 2026 GMT
  host: join.remax.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Re Max Canada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RE/MAX Canada, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RE/MAX Canada
provider_slug: re-max-canada
slug: re-max-canada-domain-security
source_filename: re-max-canada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.remax.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\n- host: blog.remax.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:51:50 2026 GMT\n  hsts: false\n  note: >-\n    The API host (baseURL https://blog.remax.ca/wp-json). Probed by hand this\n    round because the mechanical sweep did not include it. WordPress VIP nginx;\n    no Strict-Transport-Security header returned.\n- host: agentbrokerhub.remax.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:07:01 2026 GMT\n  hsts: false\n  note: >-\n    Real WordPress VIP host discovered this round (CNAME\n    remax-promotions.go-vip.net), distinct from the remax.ca DNS wildcard.\n- host: franchise.remax.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 22:54:22 2026 GMT\n  hsts: false\n- host: join.remax.ca\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 00:52:21 2026 GMT\n  hsts: false\ndomains:\n- domain: remax.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/re-max-canada/refs/heads/main/security/re-max-canada-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real-Estate
- Canada
- Brokerage
- Property Listings
- MLS
- RESO
- IDX
- PropTech
- Land Registry
- Valuation
- Rentals
- Franchising
---
