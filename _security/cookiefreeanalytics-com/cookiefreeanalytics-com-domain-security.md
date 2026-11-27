---
api_specs:
- filename: cookiefreeanalytics-com-sites-api-openapi.yml
  format: yaml
  label: Cookie Free Analytics Sites API
  slug: cookiefreeanalytics-com-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cookiefreeanalytics-com/openapi/cookiefreeanalytics-com-sites-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cookiefreeanalytics.com
  spf: true
hosts:
- cert_expires: Jan 15 19:18:53 2027 GMT
  host: cookiefreeanalytics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cookie Free Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cookie Free Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cookie Free Analytics
provider_slug: cookiefreeanalytics-com
slug: cookiefreeanalytics-com-domain-security
source_filename: cookiefreeanalytics-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cookiefreeanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 19:18:53 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cookiefreeanalytics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cookiefreeanalytics-com/security/cookiefreeanalytics-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Analytics
- Web Analytics
- Privacy
- Cookieless
- GDPR
- MCP
- Uptime Monitoring
---
