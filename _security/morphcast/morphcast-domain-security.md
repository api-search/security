---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: morphcast.com
  spf: true
hosts:
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: www.morphcast.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Morphcast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MorphCast, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MorphCast
provider_slug: morphcast
slug: morphcast-domain-security
source_filename: morphcast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.morphcast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: morphcast.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morphcast/refs/heads/main/security/morphcast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Emotion AI
- Facial Analysis
- SDK
---
