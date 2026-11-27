---
api_specs:
- filename: netzhandwerker-de-document-api-openapi.yml
  format: yaml
  label: Netz Handwerker Document API
  slug: netzhandwerker-de-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netzhandwerker-de/openapi/netzhandwerker-de-document-api-openapi.yml
- filename: netzhandwerker-de-health-api-openapi.yml
  format: yaml
  label: Netz Handwerker Health API
  slug: netzhandwerker-de-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netzhandwerker-de/openapi/netzhandwerker-de-health-api-openapi.yml
- filename: netzhandwerker-de-ocr-api-openapi.yml
  format: yaml
  label: Netz Handwerker Ocr API
  slug: netzhandwerker-de-ocr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netzhandwerker-de/openapi/netzhandwerker-de-ocr-api-openapi.yml
- filename: netzhandwerker-de-pricing-api-openapi.yml
  format: yaml
  label: Netz Handwerker Pricing API
  slug: netzhandwerker-de-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netzhandwerker-de/openapi/netzhandwerker-de-pricing-api-openapi.yml
- filename: netzhandwerker-de-readiness-api-openapi.yml
  format: yaml
  label: Netz Handwerker Readiness API
  slug: netzhandwerker-de-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netzhandwerker-de/openapi/netzhandwerker-de-readiness-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: netzhandwerker.de
  spf: true
hosts:
- cert_expires: Jan 17 01:56:12 2027 GMT
  host: netzhandwerker.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Netz Handwerker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netz Handwerker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Netz Handwerker
provider_slug: netzhandwerker-de
slug: netzhandwerker-de-domain-security
source_filename: netzhandwerker-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netzhandwerker.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 01:56:12 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: netzhandwerker.de\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/netzhandwerker-de/security/netzhandwerker-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IT
- Software Development
- AI Automation
- Sensor Solutions
---
