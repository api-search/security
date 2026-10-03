---
api_specs:
- filename: arctop-arctop-api-api-openapi.yml
  format: yaml
  label: Arctop Arctop API
  slug: arctop-arctop-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arctop/refs/heads/main/openapi/arctop-arctop-api-api-openapi.yml
- filename: arctop-dev-api-openapi.yml
  format: yaml
  label: Arctop Dev API
  slug: arctop-dev-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arctop/refs/heads/main/openapi/arctop-dev-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arctop.com
  spf: true
hosts:
- cert_expires: Dec 10 06:29:24 2026 GMT
  host: arctop.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arctop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arctop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Arctop
provider_slug: arctop
slug: arctop-domain-security
source_filename: arctop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arctop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:29:24 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: arctop.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arctop/refs/heads/main/security/arctop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Brain-Computer Interface
- Neural Data
- API Platform
- Healthcare
- Research
---
