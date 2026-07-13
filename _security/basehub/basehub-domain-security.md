---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: basehub.com
  spf: true
hosts:
- cert_expires: Aug 12 10:01:43 2026 GMT
  host: basehub.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 16:42:53 2026 GMT
  host: docs.basehub.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 22:47:48 2026 GMT
  host: api.basehub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Basehub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BaseHub, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BaseHub
provider_slug: basehub
slug: basehub-domain-security
source_filename: basehub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: basehub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 10:01:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.basehub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:42:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.basehub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:47:48 2026 GMT\n  hsts: null\ndomains:\n- domain: basehub.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basehub/refs/heads/main/security/basehub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GraphQL
- Headless CMS
- Content Management
- AI-Native
- TypeScript
---
