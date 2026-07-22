---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: forvia.com
  spf: true
hosts:
- cert_expires: Aug 27 06:53:54 2026 GMT
  host: www.forvia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forvia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forvia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Forvia
provider_slug: forvia
slug: forvia-domain-security
source_filename: forvia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.forvia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 06:53:54 2026 GMT\n  hsts: null\ndomains:\n- domain: forvia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forvia/refs/heads/main/security/forvia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Tier 1 Supplier
- Seating
- Interiors
- Lighting
- Electronics
---
