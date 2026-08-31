---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trupanion.com
  spf: true
hosts:
- cert_expires: Aug 17 20:51:38 2026 GMT
  host: www.trupanion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 04:10:01 2026 GMT
  host: api-documentation.trupanion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 09:09:04 2026 GMT
  host: vet.trupanion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trupanion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trupanion, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trupanion
provider_slug: trupanion
slug: trupanion-domain-security
source_filename: trupanion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trupanion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 20:51:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-documentation.trupanion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 04:10:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vet.trupanion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 09:09:04 2026 GMT\n  hsts: false\ndomains:\n- domain: trupanion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trupanion/refs/heads/main/security/trupanion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pet Insurance
- Insurance
- Veterinary
- InsurTech
- Direct Pay
- Partner API
---
