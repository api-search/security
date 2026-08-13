---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zetaglobal.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:zones@sailthru.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sailthru.com
  spf: true
hosts:
- cert_expires: Sep 15 05:42:27 2026 GMT
  host: zetaglobal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: products.zetaglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: api.sailthru.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sailthru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sailthru, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sailthru
provider_slug: sailthru
slug: sailthru-domain-security
source_filename: sailthru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zetaglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:42:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: products.zetaglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: false\n- host: api.sailthru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: zetaglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sailthru.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:zones@sailthru.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sailthru/refs/heads/main/security/sailthru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email Marketing
- Marketing Automation
- Personalization
- Customer Data Platform
- Transactional Email
- SMS
- Push Notifications
- Retail
- Media and Publishing
---
