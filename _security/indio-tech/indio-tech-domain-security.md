---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: useindio.com
  spf: true
hosts:
- cert_expires: Sep 24 16:27:22 2026 GMT
  host: www.useindio.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 04:18:06 2026 GMT
  host: help.useindio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Indio Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indio Technologies, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Indio Technologies
provider_slug: indio-tech
slug: indio-tech-domain-security
source_filename: indio-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.useindio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:27:22 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: help.useindio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:18:06 2026 GMT\n  hsts: null\ndomains:\n- domain: useindio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indio-tech/refs/heads/main/security/indio-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Insurance Applications
- Submissions
- Digital Forms
- ACORD
- E-Signature
- Commercial Insurance
- Applied Systems
- Partner API
---
