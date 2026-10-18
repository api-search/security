---
api_specs:
- filename: prospectapis-health-api-openapi.yml
  format: yaml
  label: ProspectAPIs Health API
  slug: prospectapis-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prospectapis/refs/heads/main/openapi/prospectapis-health-api-openapi.yml
- filename: prospectapis-pricing-api-openapi.yml
  format: yaml
  label: ProspectAPIs Pricing API
  slug: prospectapis-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prospectapis/refs/heads/main/openapi/prospectapis-pricing-api-openapi.yml
- filename: prospectapis-prospectapis-api-api-openapi.yml
  format: yaml
  label: ProspectAPIs ProspectAPIs API
  slug: prospectapis-prospectapis-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prospectapis/refs/heads/main/openapi/prospectapis-prospectapis-api-api-openapi.yml
- filename: prospectapis-watchlists-api-openapi.yml
  format: yaml
  label: ProspectAPIs Watchlists API
  slug: prospectapis-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prospectapis/refs/heads/main/openapi/prospectapis-watchlists-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prospectapis.com
  spf: true
hosts:
- cert_expires: Dec 31 03:44:00 2026 GMT
  host: prospectapis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prospectapis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProspectAPIs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ProspectAPIs
provider_slug: prospectapis
slug: prospectapis-domain-security
source_filename: prospectapis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prospectapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 03:44:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: prospectapis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prospectapis/refs/heads/main/security/prospectapis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Funding
- Research
- Data
---
