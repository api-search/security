---
api_specs:
- filename: pacer-authentication-api-openapi.yml
  format: yaml
  label: PACER Authentication API
  slug: pacer-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/administrative-office-of-the-u-s-courts/refs/heads/main/openapi/pacer-authentication-api-openapi.yml
- filename: pacer-case-locator-pcl-api-openapi.yml
  format: yaml
  label: PACER Case Locator (PCL) API
  slug: pacer-case-locator-pcl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/administrative-office-of-the-u-s-courts/refs/heads/main/openapi/pacer-case-locator-pcl-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uscourts.gov
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: www.uscourts.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: pacer.uscourts.gov
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: qa-pcl.uscourts.gov
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Administrative Office Of The U S Courts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Administrative Office of the U.S. Courts, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Administrative Office of the U.S. Courts
provider_slug: administrative-office-of-the-u-s-courts
slug: administrative-office-of-the-u-s-courts-domain-security
source_filename: administrative-office-of-the-u-s-courts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uscourts.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pacer.uscourts.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: qa-pcl.uscourts.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: uscourts.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/administrative-office-of-the-u-s-courts/refs/heads/main/security/administrative-office-of-the-u-s-courts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Courts
- Federal Government
- Legal
- PACER
- Case Records
- Judiciary
- Open Data
---
