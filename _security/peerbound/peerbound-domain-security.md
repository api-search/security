---
api_specs:
- filename: peerbound-activities-api-openapi.yml
  format: yaml
  label: Peerbound Activities API
  slug: peerbound-activities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-activities-api-openapi.yml
- filename: peerbound-moments-api-openapi.yml
  format: yaml
  label: Peerbound Moments API
  slug: peerbound-moments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-moments-api-openapi.yml
- filename: peerbound-notes-api-openapi.yml
  format: yaml
  label: Peerbound Notes API
  slug: peerbound-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-notes-api-openapi.yml
- filename: peerbound-reviews-api-openapi.yml
  format: yaml
  label: Peerbound Reviews API
  slug: peerbound-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-reviews-api-openapi.yml
- filename: peerbound-stories-api-openapi.yml
  format: yaml
  label: Peerbound Stories API
  slug: peerbound-stories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peerbound/openapi/peerbound-stories-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: peerbound.com
  spf: true
hosts:
- cert_expires: Jan 21 06:46:45 2027 GMT
  host: www.peerbound.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Peerbound Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peerbound, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Peerbound
provider_slug: peerbound
slug: peerbound-domain-security
source_filename: peerbound-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peerbound.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 06:46:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: peerbound.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/peerbound/security/peerbound-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SaaS
- Sales Enablement
- Customer Proof
- Analytics
---
