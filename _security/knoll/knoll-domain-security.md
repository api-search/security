---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: knoll.com
  spf: true
hosts:
- cert_expires: Oct  2 16:42:11 2026 GMT
  host: www.knoll.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.knoll.com
  https: false
- host: api.knoll.com
  https: false
kind: domain-security
layout: security
method: probed
name: Knoll Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knoll Inc, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Knoll Inc
provider_slug: knoll
slug: knoll-domain-security
source_filename: knoll-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.knoll.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:42:11 2026 GMT\n  hsts: false\n- host: developer.knoll.com\n  https: false\n- host: api.knoll.com\n  https: false\ndomains:\n- domain: knoll.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knoll/refs/heads/main/security/knoll-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Furniture
- Design
- Office
---
