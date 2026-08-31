---
api_specs:
- filename: kallyope-discovery-api-openapi.yml
  format: yaml
  label: Kallyope Discovery API
  slug: kallyope-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/openapi/kallyope-discovery-api-openapi.yml
- filename: kallyope-documents-api-openapi.yml
  format: yaml
  label: Kallyope Documents API
  slug: kallyope-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/openapi/kallyope-documents-api-openapi.yml
- filename: kallyope-media-api-openapi.yml
  format: yaml
  label: Kallyope Media API
  slug: kallyope-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/openapi/kallyope-media-api-openapi.yml
- filename: kallyope-news-api-openapi.yml
  format: yaml
  label: Kallyope News API
  slug: kallyope-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/openapi/kallyope-news-api-openapi.yml
- filename: kallyope-pages-api-openapi.yml
  format: yaml
  label: Kallyope Pages API
  slug: kallyope-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/openapi/kallyope-pages-api-openapi.yml
- filename: kallyope-taxonomies-api-openapi.yml
  format: yaml
  label: Kallyope Taxonomies API
  slug: kallyope-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/openapi/kallyope-taxonomies-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kallyope.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
hosts:
- cert_expires: Sep 16 12:28:12 2026 GMT
  host: kallyope.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 20:15:48 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kallyope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kallyope, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kallyope
provider_slug: kallyope
slug: kallyope-domain-security
source_filename: kallyope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kallyope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 12:28:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:15:48 2026 GMT\n  hsts: null\ndomains:\n- domain: kallyope.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kallyope/refs/heads/main/security/kallyope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Pharmaceuticals
- Drug Discovery
- Neuroscience
- Gut-Brain Axis
- Migraine
- Metabolic Disease
- Clinical Trials
- Content
---
