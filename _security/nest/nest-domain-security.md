---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nest.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Oct 10 11:53:42 2026 GMT
  host: nest.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:37:24 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:39:19 2026 GMT
  host: smartdevicemanagement.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nest, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nest
provider_slug: nest
slug: nest-domain-security
source_filename: nest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 11:53:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:37:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: smartdevicemanagement.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:39:19 2026 GMT\n  hsts: null\ndomains:\n- domain: nest.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nest/refs/heads/main/security/nest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hardware
- Smart Home
- IoT
- Home Automation
- Thermostat
- Google
- Device Access
---
