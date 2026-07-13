---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: conduent.com
  spf: true
hosts:
- cert_expires: Sep 30 19:13:00 2026 GMT
  host: www.conduent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.conduent.com
  https: false
- host: api.conduent.com
  https: false
kind: domain-security
layout: security
method: probed
name: Conduent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conduent, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Conduent
provider_slug: conduent
slug: conduent-domain-security
source_filename: conduent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conduent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:13:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.conduent.com\n  https: false\n- host: api.conduent.com\n  https: false\ndomains:\n- domain: conduent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conduent/refs/heads/main/security/conduent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Process Services
- Technology
---
