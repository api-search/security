---
api_specs:
- filename: gigsky-openapi.yml
  format: yaml
  label: GigSky Plans & Catalog API
  slug: gigsky-plans-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gigsky/refs/heads/main/openapi/gigsky-openapi.yml
- filename: gigsky-openapi.yml
  format: yaml
  label: GigSky eSIM Provisioning API
  slug: gigsky-esim-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gigsky/refs/heads/main/openapi/gigsky-openapi.yml
- filename: gigsky-openapi.yml
  format: yaml
  label: GigSky Orders API
  slug: gigsky-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gigsky/refs/heads/main/openapi/gigsky-openapi.yml
- filename: gigsky-openapi.yml
  format: yaml
  label: GigSky Usage API
  slug: gigsky-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gigsky/refs/heads/main/openapi/gigsky-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gigsky.com
  spf: true
hosts:
- cert_expires: Sep 16 17:40:07 2026 GMT
  host: www.gigsky.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.gigsky.com
  https: false
kind: domain-security
layout: security
method: probed
name: Gigsky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GigSky, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GigSky
provider_slug: gigsky
slug: gigsky-domain-security
source_filename: gigsky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gigsky.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 17:40:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gigsky.com\n  https: false\ndomains:\n- domain: gigsky.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigsky/refs/heads/main/security/gigsky-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eSIM
- Mobile Data
- Roaming
- Connectivity
- IoT
- Telecom
---
