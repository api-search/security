---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: animoto.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: animoto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- auth_challenge: Basic realm="Application"
  cert_expires: Nov 10 13:26:47 2026 GMT
  host: api.animoto.com
  hsts: max-age=15724800; includeSubDomains
  hsts_include_subdomains: true
  hsts_max_age: 15724800
  https: true
  note: 'HSTS corrected by hand on 2026-08-13. probe-domain-security.py recorded hsts: null for this host, but `curl -sI https://api.animoto.com/` and `.../jobs/` both return `strict-transport-security: max-age=15724800; includeSubDomains`. The host answers every path with HTTP 401 and an HTTP Basic challenge, which is likely why the automated probe did not capture the header.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Animoto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Animoto, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Animoto
provider_slug: animoto
slug: animoto-domain-security
source_filename: animoto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: animoto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\n- host: api.animoto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 13:26:47 2026 GMT\n  hsts: 'max-age=15724800; includeSubDomains'\n  hsts_max_age: 15724800\n  hsts_include_subdomains: true\n  auth_challenge: 'Basic realm=\"Application\"'\n  note: >-\n    HSTS corrected by hand on 2026-08-13. probe-domain-security.py recorded hsts: null for this\n    host, but `curl -sI https://api.animoto.com/` and `.../jobs/` both return\n    `strict-transport-security: max-age=15724800; includeSubDomains`. The host answers every path\n    with HTTP 401 and an HTTP Basic challenge, which is likely why the automated probe did not\n    capture the header.\ndomains:\n- domain: animoto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/animoto/refs/heads/main/security/animoto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Video
- Video Creation
- Video Editing
- Slideshow
- Marketing
- Social Media
- Content Creation
- SaaS
---
