---
api_specs:
- filename: incident-io-openapi.yml
  format: yaml
  label: Incident.io
  slug: incident-io
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incident-io/refs/heads/main/openapi/incident-io-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:infrastructure-notifications@incident.io"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: incident.io
  spf: true
hosts:
- cert_expires: Aug 17 09:35:32 2026 GMT
  host: incident.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 09:27:44 2026 GMT
  host: api.incident.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Incident Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Incident.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Incident.io
provider_slug: incident-io
slug: incident-io-domain-security
source_filename: incident-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: incident.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 09:35:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.incident.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 09:27:44 2026 GMT\n  hsts: null\ndomains:\n- domain: incident.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:infrastructure-notifications@incident.io\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incident-io/refs/heads/main/security/incident-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIOps
- Incident Management
---
