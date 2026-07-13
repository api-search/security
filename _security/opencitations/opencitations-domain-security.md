---
api_specs:
- filename: index-api.yml
  format: yaml
  label: OpenCitations Index API
  slug: opencitations-index-api
  spec_type: OpenAPI
  url: https://kinlane.github.io/all/opencitations/openapi/index-api.yml
- filename: meta-api.yml
  format: yaml
  label: OpenCitations Meta API
  slug: opencitations-meta-api
  spec_type: OpenAPI
  url: https://kinlane.github.io/all/opencitations/openapi/meta-api.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opencitations.net
  spf: true
hosts:
- cert_expires: Sep  8 06:53:26 2026 GMT
  host: api.opencitations.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 23:02:50 2026 GMT
  host: sparql.opencitations.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opencitations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenCitations, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenCitations
provider_slug: opencitations
slug: opencitations-domain-security
source_filename: opencitations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.opencitations.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 06:53:26 2026 GMT\n  hsts: false\n- host: sparql.opencitations.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:02:50 2026 GMT\n  hsts: false\ndomains:\n- domain: opencitations.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/security/opencitations-domain-security.yml
summary_line: TLSv1.3
tags:
- Citations
- Scholarly
- Research
- Open Science
- Bibliometrics
- DOI
- Academic
---
