---
api_specs:
- filename: spoolman-openapi-generated.yml
  format: yaml
  label: Spoolman API
  slug: spoolman-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spoolman/openapi/_ae-authored/spoolman-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: octoeverywhere.com
  spf: true
hosts:
- cert_expires: Jan 25 22:20:39 2027 GMT
  host: docs.octoeverywhere.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 06:23:03 2026 GMT
  host: octoeverywhere.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Spoolman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spoolman, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Spoolman
provider_slug: spoolman
slug: spoolman-domain-security
source_filename: spoolman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.octoeverywhere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 22:20:39 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: octoeverywhere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 06:23:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: octoeverywhere.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/spoolman/security/spoolman-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- 3D-printing
- inventory
- open-source
- filament
- API
---
