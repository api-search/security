---
api_specs:
- filename: uptime-com-checks-api-openapi.yml
  format: yaml
  label: Uptime.com Checks API
  slug: uptime-com-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-checks-api-openapi.yml
- filename: uptime-com-contacts-api-openapi.yml
  format: yaml
  label: Uptime.com Contacts API
  slug: uptime-com-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-contacts-api-openapi.yml
- filename: uptime-com-integrations-api-openapi.yml
  format: yaml
  label: Uptime.com Integrations API
  slug: uptime-com-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-integrations-api-openapi.yml
- filename: uptime-com-outages-api-openapi.yml
  format: yaml
  label: Uptime.com Outages API
  slug: uptime-com-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-outages-api-openapi.yml
- filename: uptime-com-sla-reports-api-openapi.yml
  format: yaml
  label: Uptime.com SLA Reports API
  slug: uptime-com-sla-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-sla-reports-api-openapi.yml
- filename: uptime-com-status-pages-api-openapi.yml
  format: yaml
  label: Uptime.com Status Pages API
  slug: uptime-com-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-status-pages-api-openapi.yml
- filename: uptime-com-tags-api-openapi.yml
  format: yaml
  label: Uptime.com Tags API
  slug: uptime-com-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-tags-api-openapi.yml
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
