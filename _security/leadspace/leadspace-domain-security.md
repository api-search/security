---
api_specs:
- filename: leadspace-enrichment-openapi.yml
  format: yaml
  label: Leadspace Enrichment API
  slug: leadspace-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-enrichment-openapi.yml
- filename: leadspace-discovery-openapi.yml
  format: yaml
  label: Leadspace Discovery API
  slug: leadspace-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-discovery-openapi.yml
- filename: leadspace-intent-openapi.yml
  format: yaml
  label: Leadspace Intent Only API
  slug: leadspace-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-intent-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leadspace.com
  spf: true
hosts:
- cert_expires: Oct 14 09:04:43 2026 GMT
  host: www.leadspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 23:39:57 2026 GMT
  host: support.leadspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: apigw.leadspace.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leadspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leadspace, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Leadspace
provider_slug: leadspace
slug: leadspace-domain-security
source_filename: leadspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leadspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 09:04:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.leadspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 23:39:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apigw.leadspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: leadspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/security/leadspace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B Data
- Customer Data Platform
- Data Enrichment
- Intent Data
- Sales Intelligence
- Account-Based Marketing
- Identity Resolution
- Firmographics
- Lead Scoring
- Company
---
