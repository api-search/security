---
api_specs:
- filename: cloud-academy-openapi-original.json
  format: json
  label: QA API (Cloud Academy)
  slug: qa-api-cloud-academy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-academy/refs/heads/main/openapi/cloud-academy-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudacademy.com
  spf: true
- caa:
  - 5 issue "godaddy.com"
  - 1 issue "letsencrypt.org"
  - 4 issue "certainly.com"
  - 0 issue "sectigo.com"
  - 2 issue "pki.goog"
  - 3 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qa.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: cloudacademy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: platform.qa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloud Academy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloud Academy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cloud Academy
provider_slug: cloud-academy
slug: cloud-academy-domain-security
source_filename: cloud-academy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudacademy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.qa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudacademy.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: qa.com\n  dnssec: false\n  caa:\n  - 5 issue \"godaddy.com\"\n  - 1 issue \"letsencrypt.org\"\n  - 4 issue \"certainly.com\"\n  - 0 issue \"sectigo.com\"\n  - 2 issue \"pki.goog\"\n  - 3 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud-academy/refs/heads/main/security/cloud-academy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Training
- Education
- Learning Management
- Cloud Computing
- Skills
- Reporting
- eLearning
---
