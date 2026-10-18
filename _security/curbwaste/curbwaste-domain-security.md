---
api_specs:
- filename: curbwaste-catalog-api-openapi.yml
  format: yaml
  label: Curbwaste Catalog API
  slug: curbwaste-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curbwaste/refs/heads/main/openapi/curbwaste-catalog-api-openapi.yml
- filename: curbwaste-customers-api-openapi.yml
  format: yaml
  label: Curbwaste Customers API
  slug: curbwaste-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curbwaste/refs/heads/main/openapi/curbwaste-customers-api-openapi.yml
- filename: curbwaste-locations-api-openapi.yml
  format: yaml
  label: Curbwaste Locations API
  slug: curbwaste-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curbwaste/refs/heads/main/openapi/curbwaste-locations-api-openapi.yml
- filename: curbwaste-zones-api-openapi.yml
  format: yaml
  label: Curbwaste Zones API
  slug: curbwaste-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curbwaste/refs/heads/main/openapi/curbwaste-zones-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: curbwaste.com
  spf: true
hosts:
- cert_expires: Dec 13 09:07:15 2026 GMT
  host: www.curbwaste.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curbwaste Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curbwaste, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Curbwaste
provider_slug: curbwaste
slug: curbwaste-domain-security
source_filename: curbwaste-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.curbwaste.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 09:07:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: curbwaste.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curbwaste/refs/heads/main/security/curbwaste-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Waste
- Software
- Software-as-a-Service
- Logistics
- Haulers
---
