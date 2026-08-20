---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 iodef "mailto:admin@movableink.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: movableink.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: movableink-dmz.com
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: movableink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: collector.movableink-dmz.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: app.movableink.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Movable Ink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Movable Ink, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Movable Ink
provider_slug: movable-ink
slug: movable-ink-domain-security
source_filename: movable-ink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: movableink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: collector.movableink-dmz.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\n- host: app.movableink.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: movableink.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 iodef \"mailto:admin@movableink.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: movableink-dmz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/movable-ink/refs/heads/main/security/movable-ink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Personalization
- Email
- Customer Data
- Mobile SDK
- Artificial Intelligence
- Advertising Technology
- Content
- Event
---
