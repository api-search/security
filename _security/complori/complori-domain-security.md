---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: complori.com
  spf: true
hosts:
- cert_expires: Aug 28 11:47:18 2026 GMT
  host: complori.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Complori Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Complori, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Complori
provider_slug: complori
slug: complori-domain-security
source_filename: complori-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: complori.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 11:47:18 2026 GMT\n  hsts: false\ndomains:\n- domain: complori.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/complori/refs/heads/main/security/complori-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- EdTech
- Online Learning
- Coding
- Programming
- Kids
- Germany
---
