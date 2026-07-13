---
api_specs:
- filename: cancer-gov-openapi.yml
  format: yaml
  label: NCI Clinical Trials Search API
  slug: clinical-trials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "identrust.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "entrust.net"
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
- host: api.cancer.gov
  https: false
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: clinicaltrialsapi.cancer.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cancer Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cancer.gov, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cancer.gov
provider_slug: cancer-gov
slug: cancer-gov-domain-security
source_filename: cancer-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cancer.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 12:17:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cancer.gov\n  https: false\n- host: clinicaltrialsapi.cancer.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cancer.gov\n  dnssec: true\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"identrust.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/security/cancer-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cancer
- Federal Government
- Healthcare
- Research
- Clinical Trials
- Genomics
- Surveillance
- Open Data
---
