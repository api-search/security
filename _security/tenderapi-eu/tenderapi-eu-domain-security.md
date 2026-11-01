---
api_specs:
- filename: tenderapi-eu-organisations-api-openapi.yml
  format: yaml
  label: tenderapi-eu Organisations API
  slug: tenderapi-eu-organisations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderapi-eu/openapi/tenderapi-eu-organisations-api-openapi.yml
- filename: tenderapi-eu-tenders-api-openapi.yml
  format: yaml
  label: tenderapi-eu Tenders API
  slug: tenderapi-eu-tenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderapi-eu/openapi/tenderapi-eu-tenders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tenderapi.eu
  spf: true
hosts:
- cert_expires: Jan  3 04:29:36 2027 GMT
  host: tenderapi.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tenderapi Eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tenderapi-eu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: tenderapi-eu
provider_slug: tenderapi-eu
slug: tenderapi-eu-domain-security
source_filename: tenderapi-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tenderapi.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 04:29:36 2027 GMT\n  hsts: false\ndomains:\n- domain: tenderapi.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tenderapi-eu/security/tenderapi-eu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- EU
- Procurement
- Tenders
- API
- Data
---
