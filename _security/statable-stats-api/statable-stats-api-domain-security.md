---
api_specs:
- filename: statable-stats-api-openapi.yml
  format: yaml
  label: Statable Stats API
  slug: statable-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statable-stats-api/refs/heads/main/openapi/statable-stats-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: statable.com
  spf: true
hosts:
- cert_expires: Nov 19 21:03:07 2026 GMT
  host: statable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 16:02:59 2026 GMT
  host: dev.statable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Statable Stats Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Statable Stats API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Statable Stats API
provider_slug: statable-stats-api
slug: statable-stats-api-domain-security
source_filename: statable-stats-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: statable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 21:03:07 2026 GMT\n  hsts: false\n- host: dev.statable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 16:02:59 2026 GMT\n  hsts: false\ndomains:\n- domain: statable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statable-stats-api/refs/heads/main/security/statable-stats-api-domain-security.yml
summary_line: TLSv1.3
tags:
- Analytics
- Web Analytics
- Cookieless
- Privacy
- GDPR
- OpenAPI
- MCP
- llms-txt
- EU-hosted
---
