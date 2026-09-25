---
api_specs:
- filename: steadyapi-collection.json
  format: json
  label: SteadyAPI
  slug: steadyapi
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/steadyapi/refs/heads/main/postman/steadyapi-collection.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: steadyapi.com
  spf: true
hosts:
- cert_expires: Nov  7 11:26:02 2026 GMT
  host: steadyapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 11:26:02 2026 GMT
  host: docs.steadyapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 11:26:02 2026 GMT
  host: api.steadyapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Steadyapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SteadyAPI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SteadyAPI
provider_slug: steadyapi
slug: steadyapi-domain-security
source_filename: steadyapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: steadyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 11:26:02 2026 GMT\n  hsts: false\n- host: docs.steadyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 11:26:02 2026 GMT\n  hsts: false\n- host: api.steadyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 11:26:02 2026 GMT\n  hsts: false\ndomains:\n- domain: steadyapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steadyapi/refs/heads/main/security/steadyapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data
- Finance
- Stock Market
- Social Media
- Reddit
- Data as a Service
- Web Data
- Alternative Data
---
