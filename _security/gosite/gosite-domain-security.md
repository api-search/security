---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gosite.com
  spf: true
hosts:
- cert_expires: Sep 28 01:01:08 2026 GMT
  host: www.gosite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: developers.gosite.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.developers.gosite.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gosite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoSite, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GoSite
provider_slug: gosite
slug: gosite-domain-security
source_filename: gosite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gosite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 01:01:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.gosite.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.developers.gosite.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gosite.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gosite/refs/heads/main/security/gosite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Small Business
- Local Services
- Website Builder
- Reputation Management
- Reviews
- Messaging
- Scheduling
- Appointments
- Payments
- Invoicing
- CRM
- Contact Management
- Local SEO
- Home Services
- Field Service
---
