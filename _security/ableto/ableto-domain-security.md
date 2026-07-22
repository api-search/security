---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ableto.com
  spf: true
hosts:
- cert_expires: Sep 30 08:43:49 2026 GMT
  host: www.ableto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ableto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AbleTo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AbleTo
provider_slug: ableto
slug: ableto-domain-security
source_filename: ableto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ableto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 08:43:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ableto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ableto/refs/heads/main/security/ableto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Behavioral Health
- Mental Health
- Telehealth
- Digital Health
---
