---
api_specs:
- filename: isitdownapi-com-incidents-api-openapi.yml
  format: yaml
  label: 60SecMonitor Incidents API
  slug: isitdownapi-com-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/isitdownapi-com/openapi/isitdownapi-com-incidents-api-openapi.yml
- filename: isitdownapi-com-status-api-openapi.yml
  format: yaml
  label: 60SecMonitor Status API
  slug: isitdownapi-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/isitdownapi-com/openapi/isitdownapi-com-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: isitdownapi.com
  spf: true
hosts:
- cert_expires: Jan  8 05:06:21 2027 GMT
  host: isitdownapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 60SecMonitor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 60SecMonitor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 60SecMonitor
provider_slug: isitdownapi-com
slug: isitdownapi-com-domain-security
source_filename: isitdownapi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: isitdownapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 05:06:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: isitdownapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/isitdownapi-com/security/isitdownapi-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Outage
- Real-Time
- SRE
---
