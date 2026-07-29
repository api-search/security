---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: virginaustralia.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_subdomain_policy: none
  dnssec: false
  domain: velocityfrequentflyer.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: www.virginaustralia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: www.velocityfrequentflyer.com
  hsts: false
  https: true
  note: Velocity Frequent Flyer marketing/member site. No Strict-Transport-Security response header was returned on 2026-07-28.
  tls_version: TLSv1.2
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.velocityfrequentflyer.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Resolves and serves TLS but returns 404 at root and at every discovery path probed. Undocumented internal surface; not listed as an API.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Virgin Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virgin Australia, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Virgin Australia
provider_slug: virgin-australia
slug: virgin-australia-domain-security
source_filename: virgin-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.virginaustralia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.velocityfrequentflyer.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: false\n  note: >-\n    Velocity Frequent Flyer marketing/member site. No Strict-Transport-Security\n    response header was returned on 2026-07-28.\n- host: api.velocityfrequentflyer.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    Resolves and serves TLS but returns 404 at root and at every discovery path\n    probed. Undocumented internal surface; not listed as an API.\ndomains:\n- domain: virginaustralia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n\
  \  dmarc_policy: reject\n- domain: velocityfrequentflyer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_subdomain_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virgin-australia/refs/heads/main/security/virgin-australia-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Travel
- Australia
- Aviation
- Airline
- Distribution
- GDS
- NDC
- Booking
- Loyalty
- Corporate Travel
---
