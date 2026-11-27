---
api_specs:
- filename: linklyhq-com-clicks-api-openapi.yml
  format: yaml
  label: Linkly Clicks API
  slug: linklyhq-com-clicks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linklyhq-com/openapi/linklyhq-com-clicks-api-openapi.yml
- filename: linklyhq-com-conversions-api-openapi.yml
  format: yaml
  label: Linkly Conversions API
  slug: linklyhq-com-conversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linklyhq-com/openapi/linklyhq-com-conversions-api-openapi.yml
- filename: linklyhq-com-domains-api-openapi.yml
  format: yaml
  label: Linkly Domains API
  slug: linklyhq-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linklyhq-com/openapi/linklyhq-com-domains-api-openapi.yml
- filename: linklyhq-com-links-api-openapi.yml
  format: yaml
  label: Linkly Links API
  slug: linklyhq-com-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linklyhq-com/openapi/linklyhq-com-links-api-openapi.yml
- filename: linklyhq-com-webhooks-api-openapi.yml
  format: yaml
  label: Linkly Webhooks API
  slug: linklyhq-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linklyhq-com/openapi/linklyhq-com-webhooks-api-openapi.yml
- filename: linklyhq-com-workspaces-api-openapi.yml
  format: yaml
  label: Linkly Workspaces API
  slug: linklyhq-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linklyhq-com/openapi/linklyhq-com-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: linklyhq.com
  spf: true
hosts:
- cert_expires: Jan 22 15:26:39 2027 GMT
  host: linklyhq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Linkly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linkly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Linkly
provider_slug: linklyhq-com
slug: linklyhq-com-domain-security
source_filename: linklyhq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linklyhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 15:26:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: linklyhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/linklyhq-com/security/linklyhq-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- URL Shorteners
- Link Tracking
- Analytics
- Branded Links
- QR Codes
- Company
---
