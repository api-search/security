---
api_specs:
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Assets API
  slug: mediavalet-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Categories API
  slug: mediavalet-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Attributes API
  slug: mediavalet-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Keywords API
  slug: mediavalet-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Uploads API
  slug: mediavalet-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Users API
  slug: mediavalet-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mediavalet.com
  spf: true
hosts:
- cert_expires: Sep 23 01:03:55 2026 GMT
  host: www.mediavalet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:44:50 2026 GMT
  host: docs.mediavalet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 21:31:14 2026 GMT
  host: api.mediavalet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mediavalet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MediaValet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MediaValet
provider_slug: mediavalet
slug: mediavalet-domain-security
source_filename: mediavalet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mediavalet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 01:03:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mediavalet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:44:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mediavalet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 21:31:14 2026 GMT\n  hsts: null\ndomains:\n- domain: mediavalet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/security/mediavalet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Asset Management
- DAM
- Media
- Assets
- Content
- Marketing
- Cloud Storage
---
