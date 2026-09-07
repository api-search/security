---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aakscience.com
  spf: true
hosts:
- cert_expires: Nov 24 00:11:03 2026 GMT
  host: aakscience.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 15:17:54 2026 GMT
  host: django.aakscience.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Aaktelescienceinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AAK Tele-Science, Inc., probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AAK Tele-Science, Inc.
provider_slug: aaktelescienceinc
slug: aaktelescienceinc-domain-security
source_filename: aaktelescienceinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aakscience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 00:11:03 2026 GMT\n  hsts: false\n- host: django.aakscience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 15:17:54 2026 GMT\n  hsts: null\ndomains:\n- domain: aakscience.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aaktelescienceinc/refs/heads/main/security/aaktelescienceinc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Research
- Science
- Collaboration
- Analytics
- Machine Learning
- SaaS
- Data
---
