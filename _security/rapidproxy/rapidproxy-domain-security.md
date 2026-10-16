---
api_specs:
- filename: rapidproxy-openapi-generated.yml
  format: yaml
  label: RapidProxy (RAPID TERMINAL UK NETWORK LIMITED) API
  slug: rapidproxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidproxy/refs/heads/main/openapi/_ae-authored/rapidproxy-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rapidproxy.io
  spf: true
hosts:
- cert_expires: Dec  5 13:05:17 2026 GMT
  host: www.rapidproxy.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rapidproxy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RapidProxy (RAPID TERMINAL UK NETWORK LIMITED), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: RapidProxy (RAPID TERMINAL UK NETWORK LIMITED)
provider_slug: rapidproxy
slug: rapidproxy-domain-security
source_filename: rapidproxy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rapidproxy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 13:05:17 2026 GMT\n  hsts: false\ndomains:\n- domain: rapidproxy.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidproxy/refs/heads/main/security/rapidproxy-domain-security.yml
summary_line: TLSv1.3
tags:
- Proxy
- Residential
- Scraping
- Data-Collection
- API
---
