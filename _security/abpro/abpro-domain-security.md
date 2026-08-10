---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: abpro.co
  spf: true
hosts:
- cert_expires: Oct 10 12:18:09 2026 GMT
  host: abpro.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abpro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abpro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Abpro
provider_slug: abpro
slug: abpro-domain-security
source_filename: abpro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abpro.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 12:18:09 2026 GMT\n  hsts: false\ndomains:\n- domain: abpro.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abpro/refs/heads/main/security/abpro-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Antibody Therapeutics
- Oncology
- Life Sciences
- Drug Discovery
- Clinical Stage
---
