---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ascap.com
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: ascap.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ascap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ASCAP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ASCAP
provider_slug: ascap
slug: ascap-domain-security
source_filename: ascap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ascap.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ascap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ascap/refs/heads/main/security/ascap-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Music
- Licensing
- Royalties
- Nonprofit
- Creators
---
