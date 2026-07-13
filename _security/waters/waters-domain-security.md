---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: waters.com
  spf: true
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: www.waters.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.waters.com
  https: false
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api.waters.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Waters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waters Corporation, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Waters Corporation
provider_slug: waters
slug: waters-domain-security
source_filename: waters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.waters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\n- host: developer.waters.com\n  https: false\n- host: api.waters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: waters.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waters/refs/heads/main/security/waters-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Laboratory
- Instruments
- Analytics
---
