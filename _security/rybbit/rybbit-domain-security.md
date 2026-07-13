---
api_specs:
- filename: rybbit-openapi.yml
  format: yaml
  label: Rybbit Event Tracking API
  slug: rybbit-event-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-openapi.yml
- filename: rybbit-openapi.yml
  format: yaml
  label: Rybbit Sites API
  slug: rybbit-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-openapi.yml
- filename: rybbit-openapi.yml
  format: yaml
  label: Rybbit Analytics Stats API
  slug: rybbit-analytics-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-openapi.yml
- filename: rybbit-openapi.yml
  format: yaml
  label: Rybbit Sessions & Retention API
  slug: rybbit-sessions-retention-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rybbit.io
  spf: true
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: rybbit.com
  spf: true
hosts:
- cert_expires: Sep 27 01:17:35 2026 GMT
  host: www.rybbit.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 21:48:58 2026 GMT
  host: rybbit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:44:12 2026 GMT
  host: app.rybbit.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rybbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rybbit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rybbit
provider_slug: rybbit
slug: rybbit-domain-security
source_filename: rybbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rybbit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 01:17:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rybbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:48:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.rybbit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:44:12 2026 GMT\n  hsts: false\ndomains:\n- domain: rybbit.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rybbit.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/security/rybbit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Web Analytics
- Product Analytics
- Privacy
- Open Source
- Cookieless
---
