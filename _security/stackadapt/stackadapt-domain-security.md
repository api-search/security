---
description: ''
domains:
- caa:
  - 0 issue "comodo.com"
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stackadapt.com
  spf: true
hosts:
- cert_expires: Oct  6 06:02:08 2026 GMT
  host: www.stackadapt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 06:02:08 2026 GMT
  host: docs.stackadapt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 06:02:08 2026 GMT
  host: api.stackadapt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stackadapt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StackAdapt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StackAdapt
provider_slug: stackadapt
slug: stackadapt-domain-security
source_filename: stackadapt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stackadapt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:02:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.stackadapt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:02:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stackadapt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:02:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stackadapt.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodo.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackadapt/refs/heads/main/security/stackadapt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Programmatic Advertising
- Digital Advertising
- Campaign Management
- Ad Tech
- DSP
- Demand-Side Platform
- Native Advertising
- Display Advertising
- Video Advertising
- Connected TV
- Audience Targeting
- Real-Time Bidding
- Conversion Tracking
- Performance Reporting
---
