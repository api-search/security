---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ceskatelevize.cz
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.ceskatelevize.cz
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Czech Television Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Czech Television, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Czech Television
provider_slug: czech-television
slug: czech-television-domain-security
source_filename: czech-television-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ceskatelevize.cz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ceskatelevize.cz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/czech-television/refs/heads/main/security/czech-television-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Video
- Public APIs
---
