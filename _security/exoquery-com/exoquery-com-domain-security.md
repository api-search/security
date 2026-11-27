---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: exoquery.com
  spf: false
hosts:
- cert_expires: Dec 20 20:37:50 2026 GMT
  host: exoquery.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ExoQuery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ExoQuery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: ExoQuery
provider_slug: exoquery-com
slug: exoquery-com-domain-security
source_filename: exoquery-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exoquery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 20:37:50 2026 GMT\n  hsts: false\ndomains:\n- domain: exoquery.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/exoquery-com/security/exoquery-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Kotlin
- SQL library
- Query composition
- JDBC
- R2DBC
- Android
- Native
---
