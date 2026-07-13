---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cd.foundation
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cdevents.dev
  spf: false
hosts:
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: cd.foundation
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 05:08:16 2026 GMT
  host: cdevents.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 21:52:45 2026 GMT
  host: www.jenkins.io
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Continuous Delivery Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Continuous Delivery Foundation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Continuous Delivery Foundation
provider_slug: continuous-delivery-foundation
slug: continuous-delivery-foundation-domain-security
source_filename: continuous-delivery-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cd.foundation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: cdevents.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 05:08:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.jenkins.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 19 21:52:45 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: cd.foundation\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cdevents.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/continuous-delivery-foundation/refs/heads/main/security/continuous-delivery-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- CI/CD
- DevOps
- Linux Foundation
- Open Source
---
