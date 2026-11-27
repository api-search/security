---
api_specs:
- filename: gasquebec-ca-cities-api-openapi.yml
  format: yaml
  label: Gas Québec Cities API
  slug: gasquebec-ca-cities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gasquebec-ca/openapi/gasquebec-ca-cities-api-openapi.yml
- filename: gasquebec-ca-fair-price-api-openapi.yml
  format: yaml
  label: Gas Québec Fair Price API
  slug: gasquebec-ca-fair-price-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gasquebec-ca/openapi/gasquebec-ca-fair-price-api-openapi.yml
- filename: gasquebec-ca-health-api-openapi.yml
  format: yaml
  label: Gas Québec Health API
  slug: gasquebec-ca-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gasquebec-ca/openapi/gasquebec-ca-health-api-openapi.yml
- filename: gasquebec-ca-search-api-openapi.yml
  format: yaml
  label: Gas Québec Search API
  slug: gasquebec-ca-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gasquebec-ca/openapi/gasquebec-ca-search-api-openapi.yml
- filename: gasquebec-ca-stations-api-openapi.yml
  format: yaml
  label: Gas Québec Stations API
  slug: gasquebec-ca-stations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gasquebec-ca/openapi/gasquebec-ca-stations-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@gasquebec.ca"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: gasquebec.ca
  spf: true
hosts:
- cert_expires: Feb  7 01:11:41 2027 GMT
  host: gasquebec.ca
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gas Québec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gas Québec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Gas Québec
provider_slug: gasquebec-ca
slug: gasquebec-ca-domain-security
source_filename: gasquebec-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gasquebec.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 01:11:41 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: gasquebec.ca\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@gasquebec.ca\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gasquebec-ca/security/gasquebec-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
