---
api_specs:
- filename: cloudkitchens-public-api-openapi.yml
  format: yaml
  label: CloudKitchens Public API
  slug: cloudkitchens-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkitchens/refs/heads/main/openapi/cloudkitchens-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cloudkitchens.com
  spf: true
hosts:
- cert_expires: Sep 27 21:29:22 2026 GMT
  host: www.cloudkitchens.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:37:39 2026 GMT
  host: developer-guides.cloudkitchens.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:37:39 2026 GMT
  host: api.cloudkitchens.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudkitchens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudKitchens, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CloudKitchens
provider_slug: cloudkitchens
slug: cloudkitchens-domain-security
source_filename: cloudkitchens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudkitchens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:29:22 2026 GMT\n  hsts: null\n- host: developer-guides.cloudkitchens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:37:39 2026 GMT\n  hsts: null\n- host: api.cloudkitchens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:37:39 2026 GMT\n  hsts: null\ndomains:\n- domain: cloudkitchens.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudkitchens/refs/heads/main/security/cloudkitchens-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Restaurant
- Ghost Kitchens
- Food Delivery
- Order Management
- Menu Management
- Storefront
- Delivery
- Reporting
- Loyalty
- Real Estate
---
