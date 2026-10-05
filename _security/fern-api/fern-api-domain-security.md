---
api_specs:
- filename: fern-api-ask-api-openapi.yml
  format: yaml
  label: Fern Ask API
  slug: fern-api-ask-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fern-api/refs/heads/main/openapi/fern-api-ask-api-openapi.yml
- filename: fern-api-website-sources-api-openapi.yml
  format: yaml
  label: Fern Website Sources API
  slug: fern-api-website-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fern-api/refs/heads/main/openapi/fern-api-website-sources-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: buildwithfern.com
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: buildwithfern.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 12 23:59:59 2027 GMT
  host: fai.buildwithfern.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Fern Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fern, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fern
provider_slug: fern-api
slug: fern-api-domain-security
source_filename: fern-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildwithfern.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: fai.buildwithfern.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: buildwithfern.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fern-api/refs/heads/main/security/fern-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Lifecycle
- SDK Generation
- Client Library
- API Documentation
- Developer Tools
- OpenAPI
- CLI
- Open Source
- Developer Experience
- Documentation
---
