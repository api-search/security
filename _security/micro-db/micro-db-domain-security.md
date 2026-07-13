---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: m3o.com
  spf: false
hosts:
- cert_expires: Sep 30 08:24:34 2026 GMT
  host: m3o.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Micro Db Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Micro DB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Micro DB
provider_slug: micro-db
slug: micro-db-domain-security
source_filename: micro-db-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: m3o.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 08:24:34 2026 GMT\n  hsts: false\ndomains:\n- domain: m3o.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/micro-db/refs/heads/main/security/micro-db-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Development
- Public APIs
---
