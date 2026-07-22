---
api_specs:
- filename: persistiq-openapi.yml
  format: yaml
  label: PersistIQ API
  slug: persistiq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/openapi/persistiq-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: persistiq.com
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: persistiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: api.persistiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Persistiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PersistIQ, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PersistIQ
provider_slug: persistiq
slug: persistiq-domain-security
source_filename: persistiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: persistiq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.persistiq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: persistiq.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/persistiq/refs/heads/main/security/persistiq-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Sales Engagement
- Sales
- Outbound
- Email Outreach
- CRM
- Lead Management
- Marketing
---
