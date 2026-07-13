---
api_specs:
- filename: credly-openapi.yml
  format: yaml
  label: Credly Badge Templates API
  slug: credly-badge-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
- filename: credly-openapi.yml
  format: yaml
  label: Credly Issued Badges API
  slug: credly-issued-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
- filename: credly-openapi.yml
  format: yaml
  label: Credly Organizations API
  slug: credly-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
- filename: credly-openapi.yml
  format: yaml
  label: Credly Events and Webhooks API
  slug: credly-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
- filename: credly-openapi.yml
  format: yaml
  label: Credly OBI Recipients API
  slug: credly-obi-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: credly.com
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: credly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: www.credly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: api.credly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Credly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Credly
provider_slug: credly
slug: credly-domain-security
source_filename: credly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: credly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.credly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.credly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: credly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/security/credly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Credentials
- Open Badges
- Badging
- Certifications
- Verifiable Credentials
- Pearson
---
