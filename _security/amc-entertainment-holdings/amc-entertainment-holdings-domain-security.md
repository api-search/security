---
api_specs:
- filename: amc-theatres-api-openapi.yml
  format: yaml
  label: AMC Theatres API
  slug: amc-theatres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/openapi/amc-theatres-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amctheatres.com
  spf: true
hosts:
- cert_expires: Oct  4 12:29:21 2026 GMT
  host: www.amctheatres.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 03:14:42 2026 GMT
  host: developers.amctheatres.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 03:38:08 2026 GMT
  host: api.amctheatres.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amc Entertainment Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMC Entertainment Holdings, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AMC Entertainment Holdings
provider_slug: amc-entertainment-holdings
slug: amc-entertainment-holdings-domain-security
source_filename: amc-entertainment-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amctheatres.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:29:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.amctheatres.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:14:42 2026 GMT\n  hsts: null\n- host: api.amctheatres.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:38:08 2026 GMT\n  hsts: null\ndomains:\n- domain: amctheatres.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amc-entertainment-holdings/refs/heads/main/security/amc-entertainment-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Entertainment
- Movies
- Theatres
- Showtimes
- Ticketing
- Concessions
- Loyalty
- Fortune 500
---
