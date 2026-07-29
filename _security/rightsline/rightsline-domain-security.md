---
api_specs:
- filename: overview
  format: yaml
  label: Rightsline Rights API
  slug: rights-api
  spec_type: Postman
  url: https://www.postman.com/kinlaneapi/rightsline/overview
- filename: postman.yaml
  format: yaml
  label: Rightsline Royalties API
  slug: royalties-api
  spec_type: Postman
  url: https://postman.rightsline.com/
- filename: rightsline-availability-api-openapi.yml
  format: yaml
  label: Rightsline Availability API
  slug: rightsline-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-availability-api-openapi.yml
- filename: rightsline-catalog-api-openapi.yml
  format: yaml
  label: Rightsline Catalog API
  slug: rightsline-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-catalog-api-openapi.yml
- filename: rightsline-contacts-api-openapi.yml
  format: yaml
  label: Rightsline Contacts API
  slug: rightsline-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-contacts-api-openapi.yml
- filename: rightsline-lists-api-openapi.yml
  format: yaml
  label: Rightsline Lists API
  slug: rightsline-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-lists-api-openapi.yml
- filename: rightsline-rights-api-openapi.yml
  format: yaml
  label: Rightsline Rights API
  slug: rightsline-rights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-rights-api-openapi.yml
- filename: rightsline-royalties-api-openapi.yml
  format: yaml
  label: Rightsline Royalties API
  slug: rightsline-royalties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-royalties-api-openapi.yml
- filename: rightsline-templates-api-openapi.yml
  format: yaml
  label: Rightsline Templates API
  slug: rightsline-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-templates-api-openapi.yml
- filename: rightsline-workflows-api-openapi.yml
  format: yaml
  label: Rightsline Workflows API
  slug: rightsline-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/openapi/rightsline-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rightsline.com
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.rightsline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: app.rightsline.com
  hsts: true
  hsts_max_age: 6307200
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 13:30:39 2026 GMT
  host: api-docs.rightsline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rightsline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rightsline, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rightsline
provider_slug: rightsline
slug: rightsline-domain-security
source_filename: rightsline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rightsline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.rightsline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 6307200\n- host: api-docs.rightsline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:30:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rightsline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rightsline/refs/heads/main/security/rightsline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Content Management
- Entertainment
- Media
- Rights Management
- Royalties
---
