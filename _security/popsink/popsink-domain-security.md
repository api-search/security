---
api_specs:
- filename: popsink-public-api-openapi-original.json
  format: json
  label: Popsink Public API
  slug: popsink-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popsink/refs/heads/main/openapi/popsink-public-api-openapi-original.json
- filename: popsink-onprem-api-openapi-original.json
  format: json
  label: Popsink Control Plane API
  slug: popsink-control-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popsink/refs/heads/main/openapi/popsink-onprem-api-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:ops@popsink.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: popsink.com
  spf: true
hosts:
- cert_expires: Sep 24 18:18:20 2026 GMT
  host: popsink.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Popsink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Popsink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Popsink
provider_slug: popsink
slug: popsink-domain-security
source_filename: popsink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: popsink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:18:20 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: popsink.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:ops@popsink.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/popsink/refs/heads/main/security/popsink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Change Data Capture
- Data Replication
- CDC
- Data Integration
- Real-Time Data
- Streaming
- ETL
- Database
- Data Platform
---
