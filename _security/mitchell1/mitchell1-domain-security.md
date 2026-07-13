---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mitchell1.com
  spf: true
hosts:
- cert_expires: Sep 25 19:09:02 2026 GMT
  host: mitchell1.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: testintents.mitchell1.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mitchell1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mitchell 1, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mitchell 1
provider_slug: mitchell1
slug: mitchell1-domain-security
source_filename: mitchell1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mitchell1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:09:02 2026 GMT\n  hsts: false\n- host: testintents.mitchell1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mitchell1.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mitchell1/refs/heads/main/security/mitchell1-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Repair Information
- Shop Management
- Labor Guide
- VIN Decode
- Snap-on
- Partner API
- Gated
---
