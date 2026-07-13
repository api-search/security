---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kevel.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@kevel.co"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kevel.co
  spf: true
hosts:
- cert_expires: Aug 16 14:03:14 2026 GMT
  host: www.kevel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: dev.kevel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: api.kevel.co
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kevel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kevel, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kevel
provider_slug: kevel
slug: kevel-domain-security
source_filename: kevel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kevel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 14:03:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.kevel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kevel.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kevel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kevel.co\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@kevel.co\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/security/kevel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ad Serving
- Advertising
- API-First
- Audience
- Monetization
- Reporting
---
