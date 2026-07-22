---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:security@yahooinc.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flurry.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: flurry.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Flurry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flurry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flurry
provider_slug: flurry
slug: flurry-domain-security
source_filename: flurry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flurry.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flurry.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:security@yahooinc.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flurry/refs/heads/main/security/flurry-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Analytics
- Mobile
- SDK
- Application Analytics
- Crash Reporting
- Push Notifications
- Advertising
---
