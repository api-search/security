---
api_specs:
- filename: domain-sentinel-com-lookup-api-openapi.yml
  format: yaml
  label: Domain Sentinel Lookup API
  slug: domain-sentinel-com-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domain-sentinel-com/openapi/domain-sentinel-com-lookup-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: domain-sentinel.com
  spf: true
hosts:
- cert_expires: Dec 25 23:43:22 2026 GMT
  host: domain-sentinel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domain Sentinel Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Domain Sentinel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Domain Sentinel
provider_slug: domain-sentinel-com
slug: domain-sentinel-com-domain-security
source_filename: domain-sentinel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domain-sentinel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:43:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: domain-sentinel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/domain-sentinel-com/security/domain-sentinel-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Domain Monitoring
- WHOIS Lookup
- RDAP API
- Brand Protection
- Expiry Alerts
- DNS Monitoring
---
