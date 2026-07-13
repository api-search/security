---
api_specs:
- filename: mabl-openapi.yml
  format: yaml
  label: Mabl API
  slug: mabl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/openapi/mabl-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mabl.com
  spf: true
hosts:
- cert_expires: Sep 21 00:17:03 2026 GMT
  host: www.mabl.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 05:44:53 2026 GMT
  host: mabl.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 10:49:45 2026 GMT
  host: api.mabl.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mabl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mabl, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mabl
provider_slug: mabl
slug: mabl-domain-security
source_filename: mabl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mabl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:17:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: mabl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 05:44:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.mabl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 10:49:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: mabl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mabl/refs/heads/main/security/mabl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Test Automation
- QA
- DevOps
- AI Testing
- Platform
---
