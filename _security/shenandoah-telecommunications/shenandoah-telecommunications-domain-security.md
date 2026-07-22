---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shentel.com
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: www.shentel.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shenandoah Telecommunications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shenandoah Telecommunications, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shenandoah Telecommunications
provider_slug: shenandoah-telecommunications
slug: shenandoah-telecommunications-domain-security
source_filename: shenandoah-telecommunications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shentel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: shentel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shenandoah-telecommunications/refs/heads/main/security/shenandoah-telecommunications-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Broadband
- Fiber Optic
- Internet Service Provider
- Telecommunications
---
