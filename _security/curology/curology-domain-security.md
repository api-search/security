---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: curology.com
  spf: true
hosts:
- cert_expires: Sep 15 01:57:23 2026 GMT
  host: www.curology.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Curology
provider_slug: curology
slug: curology-domain-security
source_filename: curology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.curology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:57:23 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: curology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curology/refs/heads/main/security/curology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Skincare
- Dermatology
- Telehealth
- Subscription
- Consumer
---
