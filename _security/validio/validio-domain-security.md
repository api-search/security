---
api_specs:
- filename: validio-export-api-openapi.yml
  format: yaml
  label: Validio Export API
  slug: validio-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validio/refs/heads/main/openapi/validio-export-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: validio.io
  spf: true
hosts:
- cert_expires: Dec 24 17:38:37 2026 GMT
  host: validio.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Validio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Validio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Validio
provider_slug: validio
slug: validio-domain-security
source_filename: validio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: validio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 17:38:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: validio.io\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/validio/refs/heads/main/security/validio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data Quality
- Observability
- Lineage
- Artificial Intelligence
---
