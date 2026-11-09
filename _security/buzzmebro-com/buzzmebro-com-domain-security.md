---
api_specs:
- filename: buzzmebro-com-applications-api-openapi.yml
  format: yaml
  label: BuzzMeBro Applications API
  slug: buzzmebro-com-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-applications-api-openapi.yml
- filename: buzzmebro-com-check-api-openapi.yml
  format: yaml
  label: BuzzMeBro Check API
  slug: buzzmebro-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-check-api-openapi.yml
- filename: buzzmebro-com-info-api-openapi.yml
  format: yaml
  label: BuzzMeBro Info API
  slug: buzzmebro-com-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-info-api-openapi.yml
- filename: buzzmebro-com-me-api-openapi.yml
  format: yaml
  label: BuzzMeBro Me API
  slug: buzzmebro-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-me-api-openapi.yml
- filename: buzzmebro-com-setups-api-openapi.yml
  format: yaml
  label: BuzzMeBro Setups API
  slug: buzzmebro-com-setups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-setups-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:support@buzzmebro.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: buzzmebro.com
  spf: true
hosts:
- cert_expires: Jan  5 23:06:37 2027 GMT
  host: buzzmebro.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buzzmebro Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BuzzMeBro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BuzzMeBro
provider_slug: buzzmebro-com
slug: buzzmebro-com-domain-security
source_filename: buzzmebro-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buzzmebro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:06:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buzzmebro.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:support@buzzmebro.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/buzzmebro-com/security/buzzmebro-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Buzzer
- Apartments
- Access
- Subscription
- Toronto
---
