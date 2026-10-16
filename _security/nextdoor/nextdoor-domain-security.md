---
api_specs:
- filename: nextdoor-advertising-api-openapi.yml
  format: yaml
  label: Nextdoor Advertising API
  slug: nextdoor-advertising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/openapi/nextdoor-advertising-api-openapi.yml
- filename: nextdoor-conversions-api-openapi.yml
  format: yaml
  label: Nextdoor Conversions API
  slug: nextdoor-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/openapi/nextdoor-conversions-api-openapi.yml
- filename: nextdoor-creatives-api-openapi.yml
  format: yaml
  label: Nextdoor Creatives API
  slug: nextdoor-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/openapi/nextdoor-creatives-api-openapi.yml
- filename: nextdoor-posts-api-openapi.yml
  format: yaml
  label: Nextdoor Posts API
  slug: nextdoor-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/openapi/nextdoor-posts-api-openapi.yml
- filename: nextdoor-search-api-openapi.yml
  format: yaml
  label: Nextdoor Search API
  slug: nextdoor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/openapi/nextdoor-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nextdoor.com
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: www.nextdoor.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 21:18:28 2026 GMT
  host: developer.nextdoor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Nextdoor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nextdoor, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nextdoor
provider_slug: nextdoor
slug: nextdoor-domain-security
source_filename: nextdoor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nextdoor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: developer.nextdoor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 21:18:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nextdoor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/security/nextdoor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social
- Local
- Advertising
- Community
- Sharing
---
