---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pgecorp.com
  spf: true
hosts:
- cert_expires: Aug  6 16:08:03 2026 GMT
  host: www.pgecorp.com
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pgande Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pgande, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: pgande
provider_slug: pgande
slug: pgande-domain-security
source_filename: pgande-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pgecorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  6 16:08:03 2026 GMT\n  hsts: true\n  hsts_max_age: 2628000\ndomains:\n- domain: pgecorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pgande/refs/heads/main/security/pgande-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
