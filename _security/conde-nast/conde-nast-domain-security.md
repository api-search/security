---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: condenast.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wired.com
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.condenast.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 19:34:15 2026 GMT
  host: www.wired.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: www.condenastentertainment.com
  https: false
kind: domain-security
layout: security
method: probed
name: Conde Nast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Condé Nast, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Condé Nast
provider_slug: conde-nast
slug: conde-nast-domain-security
source_filename: conde-nast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.condenast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.wired.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:34:15 2026 GMT\n  hsts: false\n- host: www.condenastentertainment.com\n  https: false\ndomains:\n- domain: condenast.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wired.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conde-nast/refs/heads/main/security/conde-nast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Media
- Publishing
- Magazines
- News
- Journalism
- RSS
- Video
- JSON-LD
- Schema.org
---
