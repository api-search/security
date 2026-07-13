---
api_specs:
- filename: completedns-v2-openapi.yml
  format: yaml
  label: CompleteDNS API v2
  slug: dns-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/completedns/refs/heads/main/openapi/completedns-v2-openapi.yml
- filename: completedns-v1-openapi.yml
  format: yaml
  label: CompleteDNS API v1
  slug: ns-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/completedns/refs/heads/main/openapi/completedns-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: completedns.com
  spf: true
hosts:
- cert_expires: Sep  4 15:28:22 2026 GMT
  host: completedns.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 15:28:22 2026 GMT
  host: api.completedns.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Completedns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CompleteDNS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CompleteDNS
provider_slug: completedns
slug: completedns-domain-security
source_filename: completedns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: completedns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:28:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.completedns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:28:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: completedns.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/completedns/refs/heads/main/security/completedns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DNS
- DNS History
- Domain Intelligence
- Domains
- Nameservers
- Threat Intelligence
---
