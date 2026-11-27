---
api_specs:
- filename: linkinseconds-com-analytics-api-openapi.yml
  format: yaml
  label: Link in Seconds Analytics API
  slug: linkinseconds-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkinseconds-com/openapi/linkinseconds-com-analytics-api-openapi.yml
- filename: linkinseconds-com-links-api-openapi.yml
  format: yaml
  label: Link in Seconds Links API
  slug: linkinseconds-com-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkinseconds-com/openapi/linkinseconds-com-links-api-openapi.yml
- filename: linkinseconds-com-status-api-openapi.yml
  format: yaml
  label: Link in Seconds Status API
  slug: linkinseconds-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkinseconds-com/openapi/linkinseconds-com-status-api-openapi.yml
- filename: linkinseconds-com-uploads-api-openapi.yml
  format: yaml
  label: Link in Seconds Uploads API
  slug: linkinseconds-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkinseconds-com/openapi/linkinseconds-com-uploads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: linkinseconds.com
  spf: true
hosts:
- cert_expires: Jan 27 03:18:08 2027 GMT
  host: linkinseconds.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Link in Seconds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Link in Seconds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Link in Seconds
provider_slug: linkinseconds-com
slug: linkinseconds-com-domain-security
source_filename: linkinseconds-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linkinseconds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 03:18:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: linkinseconds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/linkinseconds-com/security/linkinseconds-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- File Sharing
- Link Management
- Software-as-a-Service
- Cloud Storage
- Productivity
---
