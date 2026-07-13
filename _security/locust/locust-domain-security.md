---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: locust.io
  spf: false
hosts:
- cert_expires: Sep  1 08:53:55 2026 GMT
  host: locust.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Locust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Locust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Locust
provider_slug: locust
slug: locust-domain-security
source_filename: locust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: locust.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 08:53:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: locust.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/locust/refs/heads/main/security/locust-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Load Testing
- Performance Testing
- Open Source
- Python
- Testing
---
