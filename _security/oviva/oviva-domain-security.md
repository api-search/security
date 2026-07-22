---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oviva.com
  spf: true
hosts:
- cert_expires: Sep 27 21:31:15 2026 GMT
  host: oviva.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oviva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oviva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Oviva
provider_slug: oviva
slug: oviva-domain-security
source_filename: oviva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oviva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:31:15 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: oviva.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oviva/refs/heads/main/security/oviva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Diabetes
- Weight Management
- Nutrition
- Digital Therapeutics
- Telehealth
---
