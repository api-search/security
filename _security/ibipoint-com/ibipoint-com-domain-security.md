---
api_specs:
- filename: ibipoint-com-openapi.json
  format: json
  label: eSIM Catalog
  slug: esim-catalog
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ibipoint-com/openapi/ibipoint-com-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ibipoint.com
  spf: true
hosts:
- cert_expires: Dec 16 11:08:20 2026 GMT
  host: ibipoint.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ibiPoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ibiPoint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ibiPoint
provider_slug: ibipoint-com
slug: ibipoint-com-domain-security
source_filename: ibipoint-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ibipoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 11:08:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ibipoint.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ibipoint-com/security/ibipoint-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Travel
- eSIM
- Mobile Data
- Global
---
