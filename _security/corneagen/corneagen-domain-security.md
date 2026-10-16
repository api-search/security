---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: corneagen.com
  spf: true
hosts:
- cert_expires: Dec  6 19:51:09 2026 GMT
  host: corneagen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Corneagen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CorneaGen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CorneaGen
provider_slug: corneagen
slug: corneagen-domain-security
source_filename: corneagen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corneagen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 19:51:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: corneagen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corneagen/refs/heads/main/security/corneagen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Ophthalmology
- Surgery
- Tissue
---
