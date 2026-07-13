---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: purpleair.com
  spf: true
hosts:
- cert_expires: Aug 28 00:52:02 2026 GMT
  host: www2.purpleair.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Purple Air Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Purple Air, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Purple Air
provider_slug: purple-air
slug: purple-air-domain-security
source_filename: purple-air-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www2.purpleair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 00:52:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: purpleair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/purple-air/refs/heads/main/security/purple-air-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Science And Math
- Public APIs
---
