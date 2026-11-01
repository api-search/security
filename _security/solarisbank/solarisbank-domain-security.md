---
api_specs:
- filename: solarisbank-openapi-generated.yml
  format: yaml
  label: solarisBank AG API
  slug: solarisbank-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/solarisbank/openapi/_ae-authored/solarisbank-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: solarisbank.com
  spf: true
hosts:
- cert_expires: Jan  6 12:44:44 2027 GMT
  host: solarisbank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Solarisbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for solarisBank AG, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: solarisBank AG
provider_slug: solarisbank
slug: solarisbank-domain-security
source_filename: solarisbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: solarisbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 12:44:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: solarisbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/solarisbank/security/solarisbank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Banking-as-a-Service
- Embedded Finance
- Europe
---
