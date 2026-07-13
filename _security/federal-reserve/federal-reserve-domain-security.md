---
api_specs:
- filename: federal-reserve-fred-openapi.yml
  format: yaml
  label: Federal Reserve FRED API
  slug: federal-reserve
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-reserve/refs/heads/main/openapi/federal-reserve-fred-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: federalreserve.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stlouisfed.org
  spf: true
hosts:
- cert_expires: Sep 26 07:51:25 2026 GMT
  host: www.federalreserve.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: fred.stlouisfed.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.stlouisfed.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Federal Reserve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Reserve, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Federal Reserve
provider_slug: federal-reserve
slug: federal-reserve-domain-security
source_filename: federal-reserve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.federalreserve.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 07:51:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fred.stlouisfed.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\n- host: api.stlouisfed.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: federalreserve.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: stlouisfed.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-reserve/refs/heads/main/security/federal-reserve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Economics
- Federal Government
- Finance
---
