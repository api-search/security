---
api_specs:
- filename: lytics-accounts-api-openapi.yml
  format: yaml
  label: Lytics Accounts API
  slug: lytics-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-accounts-api-openapi.yml
- filename: lytics-connections-api-openapi.yml
  format: yaml
  label: Lytics Connections API
  slug: lytics-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-connections-api-openapi.yml
- filename: lytics-datamodels-api-openapi.yml
  format: yaml
  label: Lytics Datamodels API
  slug: lytics-datamodels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-datamodels-api-openapi.yml
- filename: lytics-entity-api-openapi.yml
  format: yaml
  label: Lytics Entity API
  slug: lytics-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-entity-api-openapi.yml
- filename: lytics-jobs-api-openapi.yml
  format: yaml
  label: Lytics Jobs API
  slug: lytics-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-jobs-api-openapi.yml
- filename: lytics-segments-api-openapi.yml
  format: yaml
  label: Lytics Segments API
  slug: lytics-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-segments-api-openapi.yml
- filename: lytics-work-api-openapi.yml
  format: yaml
  label: Lytics Work API
  slug: lytics-work-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-work-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lytics.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lytics.io
  spf: true
hosts:
- cert_expires: Sep 18 19:13:49 2026 GMT
  host: www.lytics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 11:05:35 2026 GMT
  host: docs.lytics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: api.lytics.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lytics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Lytics
provider_slug: lytics
slug: lytics-domain-security
source_filename: lytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 19:13:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.lytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 11:05:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lytics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lytics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: lytics.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/security/lytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Customer Data Platform
- CDP
- Personalization
- Segmentation
- User Profiles
- Behavioral Analytics
- Content Affinity
- Real-Time Data
- Marketing Automation
- Audience Activation
---
