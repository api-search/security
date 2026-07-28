---
api_specs:
- filename: green-button-alliance-green-button-api-openapi.yml
  format: yaml
  label: Green Button Connect My Data (CMD) ESPI Resource Server API
  slug: green-button-connect-my-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-green-button-api-openapi.yml
- filename: green-button-alliance-authorization-server-openapi.yml
  format: yaml
  label: OpenESPI Authorization Server API
  slug: openespi-authorization-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-authorization-server-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greenbuttonalliance.org
  spf: true
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sni.cloudflaressl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greenbuttondata.org
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.greenbuttonalliance.org
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 20:26:53 2026 GMT
  host: sandbox.greenbuttonalliance.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 18:43:32 2026 GMT
  host: services.greenbuttondata.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Green Button Alliance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Button Alliance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Green Button Alliance
provider_slug: green-button-alliance
slug: green-button-alliance-domain-security
source_filename: green-button-alliance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greenbuttonalliance.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: sandbox.greenbuttonalliance.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:26:53 2026 GMT\n  hsts: null\n- host: services.greenbuttondata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 18:43:32 2026 GMT\n  hsts: false\ndomains:\n- domain: greenbuttonalliance.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: greenbuttondata.org\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sni.cloudflaressl.com\"\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/security/green-button-alliance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Utilities
- Electricity
- Gas
- Water
- Smart Metering
- Green Button
- ESPI
- Standards Body
- Certification
- Consumer Energy Data
---
