---
api_specs:
- filename: chadwin-api-openapi.json
  format: json
  label: Chadwin API API
  slug: chadwin-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chadwin/refs/heads/main/openapi/_original/chadwin-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chadwin.co
  spf: true
hosts:
- cert_expires: Jan  8 18:43:10 2027 GMT
  host: chadwin.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chadwin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chadwin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chadwin
provider_slug: chadwin
slug: chadwin-domain-security
source_filename: chadwin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chadwin.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 18:43:10 2027 GMT\n  hsts: false\ndomains:\n- domain: chadwin.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chadwin/refs/heads/main/security/chadwin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- DataAnalytics
- Integration
- APIs
- Enterprise
---
