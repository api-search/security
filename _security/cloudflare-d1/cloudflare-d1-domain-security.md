---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Cloudflare D1 API
  slug: cloudflare-d1-api
  spec_type: OpenAPI
  url: https://developers.cloudflare.com/api/resources/d1/subresources/database/
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:tls-abuse@cloudflare.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cloudflare.com
  spf: true
hosts:
- cert_expires: Oct  4 07:46:56 2026 GMT
  host: www.cloudflare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 16:43:14 2026 GMT
  host: developers.cloudflare.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:15:42 2026 GMT
  host: api.cloudflare.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudflare D1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudflare D1, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cloudflare D1
provider_slug: cloudflare-d1
slug: cloudflare-d1-domain-security
source_filename: cloudflare-d1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:46:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.cloudflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 16:43:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.cloudflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:15:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cloudflare.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:tls-abuse@cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudflare-d1/refs/heads/main/security/cloudflare-d1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Database
- SQLite
- Serverless
- Edge Computing
- SQL
- Cloudflare
- Workers
---
