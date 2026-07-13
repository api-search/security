---
api_specs:
- filename: national-cancer-institute-openapi.yml
  format: yaml
  label: NCI Genomic Data Commons API
  slug: gdc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-cancer-institute/main/openapi/national-cancer-institute-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "identrust.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cancer.gov
  spf: true
hosts:
- cert_expires: Sep  2 12:17:56 2026 GMT
  host: www.cancer.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 21 23:59:59 2027 GMT
  host: gdc.cancer.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: api.gdc.cancer.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: National Cancer Institute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Cancer Institute, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Cancer Institute
provider_slug: national-cancer-institute
slug: national-cancer-institute-domain-security
source_filename: national-cancer-institute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cancer.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 12:17:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gdc.cancer.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gdc.cancer.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cancer.gov\n  dnssec: true\n  caa:\n  - 0 issue \"identrust.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-cancer-institute/refs/heads/main/security/national-cancer-institute-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cancer
- Federal Government
- Health
- Research
---
