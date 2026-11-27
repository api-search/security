---
api_specs:
- filename: faxonline-app-fax-api-openapi.yml
  format: yaml
  label: FaxOnline Fax API
  slug: faxonline-app-fax-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faxonline-app/openapi/faxonline-app-fax-api-openapi.yml
- filename: faxonline-app-up-api-openapi.yml
  format: yaml
  label: FaxOnline Up API
  slug: faxonline-app-up-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faxonline-app/openapi/faxonline-app-up-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: faxonline.app
  spf: true
hosts:
- cert_expires: Jan  6 18:10:49 2027 GMT
  host: faxonline.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FaxOnline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FaxOnline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: FaxOnline
provider_slug: faxonline-app
slug: faxonline-app-domain-security
source_filename: faxonline-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: faxonline.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 18:10:49 2027 GMT\n  hsts: false\ndomains:\n- domain: faxonline.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/faxonline-app/security/faxonline-app-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fax
- Online
- One-Time
- US Fax
- Payments
---
