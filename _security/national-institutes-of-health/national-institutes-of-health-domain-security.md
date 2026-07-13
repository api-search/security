---
api_specs:
- filename: national-institutes-of-health-openapi.yml
  format: yaml
  label: NIH RePORTER API
  slug: reporter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-institutes-of-health/main/openapi/national-institutes-of-health-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nih.gov
  spf: true
hosts:
- cert_expires: Sep 20 12:45:50 2026 GMT
  host: www.nih.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 19:39:20 2026 GMT
  host: api.reporter.nih.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Institutes Of Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Institutes of Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Institutes of Health
provider_slug: national-institutes-of-health
slug: national-institutes-of-health-domain-security
source_filename: national-institutes-of-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:45:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.reporter.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 19:39:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nih.gov\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-institutes-of-health/refs/heads/main/security/national-institutes-of-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Health
- Research
- Funding
- Publications
---
