---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 iodef "mailto:ts@hotdoc.com.au"
  - 0 issue "amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hotdoc.com.au
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.hotdoc.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 00:39:37 2026 GMT
  host: practices.hotdoc.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hotdoc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HotDoc, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HotDoc
provider_slug: hotdoc
slug: hotdoc-domain-security
source_filename: hotdoc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hotdoc.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: practices.hotdoc.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 00:39:37 2026 GMT\n  hsts: false\ndomains:\n- domain: hotdoc.com.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 iodef \"mailto:ts@hotdoc.com.au\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotdoc/refs/heads/main/security/hotdoc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Australia
- Patient Engagement
- Online Booking
- Appointment Scheduling
- Telehealth
- Practice Management
- Primary Care
- Digital Health
- e-Prescribing
---
