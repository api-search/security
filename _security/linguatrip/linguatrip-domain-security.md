---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: linguatrip.com
  spf: true
hosts:
- cert_expires: Sep 22 13:43:41 2026 GMT
  host: linguatrip.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linguatrip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linguatrip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Linguatrip
provider_slug: linguatrip
slug: linguatrip-domain-security
source_filename: linguatrip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linguatrip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:43:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: linguatrip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linguatrip/refs/heads/main/security/linguatrip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Language Learning
- Travel
- Online Learning
- Test Preparation
- Study Abroad
- Marketplace
---
