---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moxo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moxtra.com
  spf: true
hosts:
- cert_expires: Aug 17 01:58:17 2026 GMT
  host: www.moxo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 06:25:28 2026 GMT
  host: developer.moxtra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 28 06:25:28 2026 GMT
  host: api.moxtra.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Moxtra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moxtra, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moxtra
provider_slug: moxtra
slug: moxtra-domain-security
source_filename: moxtra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moxo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 01:58:17 2026 GMT\n  hsts: false\n- host: developer.moxtra.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 06:25:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.moxtra.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 06:25:28 2026 GMT\n  hsts: null\ndomains:\n- domain: moxo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: moxtra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moxtra/refs/heads/main/security/moxtra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Customer Engagement
- Messaging
- Video Conferencing
- Workflow
- Embedded SDK
- Communication
---
