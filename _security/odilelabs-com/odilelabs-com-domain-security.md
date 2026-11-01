---
api_specs:
- filename: odilelabs-com-account-api-openapi.yml
  format: yaml
  label: odilelabs-com Account API
  slug: odilelabs-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odilelabs-com/openapi/odilelabs-com-account-api-openapi.yml
- filename: odilelabs-com-lines-api-openapi.yml
  format: yaml
  label: odilelabs-com Lines API
  slug: odilelabs-com-lines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odilelabs-com/openapi/odilelabs-com-lines-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: odilelabs.com
  spf: true
hosts:
- cert_expires: Jan 17 04:15:06 2027 GMT
  host: odilelabs.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Odilelabs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for odilelabs-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: odilelabs-com
provider_slug: odilelabs-com
slug: odilelabs-com-domain-security
source_filename: odilelabs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: odilelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 04:15:06 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: odilelabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/odilelabs-com/security/odilelabs-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communication Infrastructure
- AI Receptionist
- Phone Answering
- Developer API
---
