---
api_specs:
- filename: democracy-works-authorities-api-openapi.yml
  format: yaml
  label: Democracy Works Authorities API
  slug: democracy-works-authorities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/openapi/democracy-works-authorities-api-openapi.yml
- filename: democracy-works-elections-api-openapi.yml
  format: yaml
  label: Democracy Works Elections API
  slug: democracy-works-elections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/openapi/democracy-works-elections-api-openapi.yml
- filename: democracy-works-exports-api-openapi.yml
  format: yaml
  label: Democracy Works Exports API
  slug: democracy-works-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/openapi/democracy-works-exports-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: democracy.works
  spf: true
hosts:
- cert_expires: Sep 29 13:41:02 2026 GMT
  host: www.democracy.works
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: data.democracy.works
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.democracy.works
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Democracy Works Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Democracy Works, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Democracy Works
provider_slug: democracy-works
slug: democracy-works-domain-security
source_filename: democracy-works-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.democracy.works\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:41:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.democracy.works\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: null\n- host: api.democracy.works\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: democracy.works\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/democracy-works/refs/heads/main/security/democracy-works-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Civic Tech
- Elections
- Government
- Nonprofit
- Voter Information
- Voting
---
