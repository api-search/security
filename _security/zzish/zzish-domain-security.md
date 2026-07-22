---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zzish.com
  spf: true
hosts:
- cert_expires: Sep 28 00:38:10 2026 GMT
  host: zzish.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zzish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zzish, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zzish
provider_slug: zzish
slug: zzish-domain-security
source_filename: zzish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zzish.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 00:38:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zzish.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zzish/refs/heads/main/security/zzish-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- K-12
- Assessment
- Quizzes
- Learning
- AI Tutoring
---
