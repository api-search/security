---
api_specs:
- filename: clerk-io-openapi.yml
  format: yaml
  label: Clerk.io API
  slug: clerk-io-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/openapi/clerk-io-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:product-devops@clerk.io"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clerk.io
  spf: true
hosts:
- cert_expires: Sep 12 06:31:50 2026 GMT
  host: www.clerk.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:42:59 2026 GMT
  host: docs.clerk.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clerk Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clerk.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clerk.io
provider_slug: clerk-io
slug: clerk-io-domain-security
source_filename: clerk-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clerk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:31:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.clerk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:42:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clerk.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:product-devops@clerk.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clerk-io/refs/heads/main/security/clerk-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Commerce
- E-Commerce
- Email Marketing
- Personalization
- Recommendations
- Search
---
