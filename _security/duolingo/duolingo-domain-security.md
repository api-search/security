---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: duolingo.com
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.duolingo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Duolingo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Duolingo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Duolingo
provider_slug: duolingo
slug: duolingo-domain-security
source_filename: duolingo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.duolingo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: duolingo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duolingo/refs/heads/main/security/duolingo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Language Learning
- Education
- EdTech
- Mobile Learning
- Gamification
- Language Assessment
- English Proficiency
- Math Learning
- Music Learning
- Early Literacy
- Consumer Apps
- Subscription
---
