---
api_specs:
- filename: opshub-openapi-generated.yml
  format: yaml
  label: OpsHub API
  slug: opshub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opshub/openapi/_ae-authored/opshub-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: opshub.com
  spf: true
hosts:
- cert_expires: Nov 26 08:14:23 2026 GMT
  host: opshub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opshub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpsHub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OpsHub
provider_slug: opshub
slug: opshub-domain-security
source_filename: opshub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opshub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 08:14:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opshub.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/opshub/security/opshub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Integration
- Migration
- ALM
- ITSM
- CRM
- DevOps
- Enterprise
---
