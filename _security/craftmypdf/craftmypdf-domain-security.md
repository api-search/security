---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: craftmypdf.com
  spf: true
hosts:
- cert_expires: Sep 25 22:48:49 2026 GMT
  host: craftmypdf.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Craftmypdf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CraftMyPDF, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CraftMyPDF
provider_slug: craftmypdf
slug: craftmypdf-domain-security
source_filename: craftmypdf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: craftmypdf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:48:49 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: craftmypdf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/craftmypdf/refs/heads/main/security/craftmypdf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Documents And Productivity
- Public APIs
---
