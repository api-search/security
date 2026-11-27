---
api_specs:
- filename: codebeamer-openapi-generated.yml
  format: yaml
  label: Codebeamer REST API (Swagger v3)
  slug: codebeamer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codebeamer/openapi/_ae-authored/codebeamer-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 128 issue "identrust.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: codebeamer.com
  spf: true
hosts:
- cert_expires: Dec 25 23:38:07 2026 GMT
  host: codebeamer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Codebeamer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codebeamer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Codebeamer
provider_slug: codebeamer
slug: codebeamer-domain-security
source_filename: codebeamer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codebeamer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:38:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: codebeamer.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 128 issue \"identrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/codebeamer/security/codebeamer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Application Lifecycle Management
- Requirements Management
- Software Engineering
- Test Management
- Risk Management
- DevOps
- PTC
---
