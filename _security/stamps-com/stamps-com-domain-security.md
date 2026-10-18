---
api_specs:
- filename: stamps-com-account-api-openapi.yml
  format: yaml
  label: Stamps.com Account API
  slug: stamps-com-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stamps-com/refs/heads/main/openapi/stamps-com-account-api-openapi.yml
- filename: stamps-com-addresses-api-openapi.yml
  format: yaml
  label: Stamps.com Addresses API
  slug: stamps-com-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stamps-com/refs/heads/main/openapi/stamps-com-addresses-api-openapi.yml
- filename: stamps-com-balance-api-openapi.yml
  format: yaml
  label: Stamps.com Balance API
  slug: stamps-com-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stamps-com/refs/heads/main/openapi/stamps-com-balance-api-openapi.yml
- filename: stamps-com-labels-api-openapi.yml
  format: yaml
  label: Stamps.com Labels API
  slug: stamps-com-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stamps-com/refs/heads/main/openapi/stamps-com-labels-api-openapi.yml
- filename: stamps-com-stamps-com-api-api-openapi.yml
  format: yaml
  label: Stamps.com Stamps.com API
  slug: stamps-com-stamps-com-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stamps-com/refs/heads/main/openapi/stamps-com-stamps-com-api-api-openapi.yml
- filename: stamps-com-tracking-api-openapi.yml
  format: yaml
  label: Stamps.com Tracking API
  slug: stamps-com-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stamps-com/refs/heads/main/openapi/stamps-com-tracking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stamps.com
  spf: true
hosts:
- cert_expires: Jan 11 04:07:31 2027 GMT
  host: www.stamps.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stamps Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stamps.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stamps.com
provider_slug: stamps-com
slug: stamps-com-domain-security
source_filename: stamps-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stamps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 04:07:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stamps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stamps-com/refs/heads/main/security/stamps-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Shipping
- E-Commerce
- Logistics
---
