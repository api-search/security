---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: flyr.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flyrhospitality.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pacerevenue.com
  spf: true
hosts:
- cert_expires: Sep  9 11:06:21 2026 GMT
  host: flyr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 09:28:24 2026 GMT
  host: developer.flyr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 04:41:40 2026 GMT
  host: www.flyrhospitality.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 19:03:36 2026 GMT
  host: api.pacerevenue.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 20:23:38 2026 GMT
  host: graphql.pacerevenue.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 21:40:29 2026 GMT
  host: legacy-api.pacerevenue.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 18:15:36 2026 GMT
  host: app.pacerevenue.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flyr Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FLYR Labs, probed live across 7 host(s) and 3 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: FLYR Labs
provider_slug: flyr-labs
slug: flyr-labs-domain-security
source_filename: flyr-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flyr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 11:06:21 2026 GMT\n  hsts: null\n- host: developer.flyr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:28:24 2026 GMT\n  hsts: null\n- host: www.flyrhospitality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:41:40 2026 GMT\n  hsts: null\n- host: api.pacerevenue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 19:03:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: graphql.pacerevenue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 20:23:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: legacy-api.pacerevenue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:40:29 2026 GMT\n  hsts: true\n  hsts_max_age:\
  \ 31536000\n  hsts_include_subdomains: true\n- host: app.pacerevenue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:15:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: false\ndomains:\n- domain: flyr.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: flyrhospitality.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pacerevenue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnotes:\n- >-\n  The four *.pacerevenue.com API/console hosts were probed by hand in the same pass (openssl s_client +\n  HEAD) because the FLYR Hospitality API tier lives on a different registrable domain than the apis.yml\n  Website host; all four set HSTS, while none of the flyr.com / flyrhospitality.com web hosts do.\n- >-\n  No CAA records are published on any of the three registrable domains. DMARC is present everywhere but\n  enforced\
  \ only on flyrhospitality.com (p=quarantine); flyr.com and pacerevenue.com are both p=none.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flyr-labs/refs/heads/main/security/flyr-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- travel-technology
- airlines
- hospitality
- revenue-management
- dynamic-pricing
- artificial-intelligence
- airline-retailing
- ndc
- offer-and-order
- hotel-technology
- forecasting
- cargo
---
