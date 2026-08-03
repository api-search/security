---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jetzero.aero
  spf: true
hosts:
- cert_expires: Sep 20 15:03:48 2026 GMT
  host: www.jetzero.aero
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jetzero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JetZero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JetZero
provider_slug: jetzero
slug: jetzero-domain-security
source_filename: jetzero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jetzero.aero\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:03:48 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\ndomains:\n- domain: jetzero.aero\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetzero/refs/heads/main/security/jetzero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Aerospace
- Aviation
- Aircraft Manufacturing
- Advanced Manufacturing
- Sustainability
- Transportation
- Defense
---
