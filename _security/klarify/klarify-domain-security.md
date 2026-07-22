---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: klarify.ca
  spf: true
hosts:
- cert_expires: Sep  3 11:01:34 2026 GMT
  host: www.klarify.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klarify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klarify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Klarify
provider_slug: klarify
slug: klarify-domain-security
source_filename: klarify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.klarify.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 11:01:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: klarify.ca\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klarify/refs/heads/main/security/klarify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Care
- Mental Health
- Artificial Intelligence
- Clinical Documentation
- Medical Records
- Insurance
- Practice Management
- Vertical SaaS
- Directory
---
