---
api_specs:
- filename: uptime-com-openapi.yml
  format: yaml
  label: Uptime.com Checks & Monitors API
  slug: checks-monitors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-openapi.yml
- filename: uptime-com-openapi.yml
  format: yaml
  label: Uptime.com Outages API
  slug: outages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-openapi.yml
- filename: uptime-com-openapi.yml
  format: yaml
  label: Uptime.com SLA Reports API
  slug: sla-reports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-openapi.yml
- filename: uptime-com-openapi.yml
  format: yaml
  label: Uptime.com Status Pages API
  slug: status-pages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-openapi.yml
- filename: uptime-com-openapi.yml
  format: yaml
  label: Uptime.com Contacts & Integrations API
  slug: contacts-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-openapi.yml
- filename: uptime-com-openapi.yml
  format: yaml
  label: Uptime.com Tags API
  slug: tags
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uptime.com
  spf: true
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: uptime.com
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uptime Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uptime.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Uptime.com
provider_slug: uptime-com
slug: uptime-com-domain-security
source_filename: uptime-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uptime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: uptime.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/security/uptime-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Uptime
- Website Monitoring
- Status Pages
- SLA
---
