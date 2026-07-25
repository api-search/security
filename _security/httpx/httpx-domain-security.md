---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: python-httpx.org
  spf: false
hosts:
- cert_expires: Sep 23 18:30:53 2026 GMT
  host: www.python-httpx.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Httpx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HTTPX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: HTTPX
provider_slug: httpx
slug: httpx-domain-security
source_filename: httpx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.python-httpx.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 18:30:53 2026 GMT\n  hsts: false\ndomains:\n- domain: python-httpx.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/httpx/refs/heads/main/security/httpx-domain-security.yml
summary_line: TLSv1.3
tags:
- Async
- Clients
- HTTP Client
- Library
- Python
---
