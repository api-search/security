---
api_specs:
- filename: nhtsa-datasets-api.json
  format: json
  label: NHTSA Datasets and APIs
  slug: nhtsa-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dot/refs/heads/main/openapi/nhtsa-datasets-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: transportation.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dot.gov
  spf: true
hosts:
- cert_expires: Jul 21 23:59:59 2026 GMT
  host: www.transportation.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: mobile.fmcsa.dot.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 21 23:59:59 2026 GMT
  host: www.fmcsa.dot.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Department of Transportation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US Department of Transportation
provider_slug: dot
slug: dot-domain-security
source_filename: dot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transportation.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 21 23:59:59 2026 GMT\n  hsts: null\n- host: mobile.fmcsa.dot.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.fmcsa.dot.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: transportation.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dot.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dot/refs/heads/main/security/dot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Transportation
- Trucking
- Aviation
- VehicleSafety
- Transit
- OpenData
---
