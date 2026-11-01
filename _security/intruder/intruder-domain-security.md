---
api_specs:
- filename: intruder-health-api-openapi.yml
  format: yaml
  label: Intruder Health API
  slug: intruder-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-health-api-openapi.yml
- filename: intruder-issues-api-openapi.yml
  format: yaml
  label: Intruder Issues API
  slug: intruder-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-issues-api-openapi.yml
- filename: intruder-licenses-api-openapi.yml
  format: yaml
  label: Intruder Licenses API
  slug: intruder-licenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-licenses-api-openapi.yml
- filename: intruder-occurrences-api-openapi.yml
  format: yaml
  label: Intruder Occurrences API
  slug: intruder-occurrences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-occurrences-api-openapi.yml
- filename: intruder-scans-api-openapi.yml
  format: yaml
  label: Intruder Scans API
  slug: intruder-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-scans-api-openapi.yml
- filename: intruder-tags-api-openapi.yml
  format: yaml
  label: Intruder Tags API
  slug: intruder-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-tags-api-openapi.yml
- filename: intruder-targets-api-openapi.yml
  format: yaml
  label: Intruder Targets API
  slug: intruder-targets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-targets-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intruder.io
  spf: true
hosts:
- cert_expires: Dec 13 15:31:36 2026 GMT
  host: intruder.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Intruder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intruder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Intruder
provider_slug: intruder
slug: intruder-domain-security
source_filename: intruder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intruder.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 15:31:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: intruder.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/intruder/security/intruder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cloud
- API
- AI
- Platform
---
