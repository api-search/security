---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dagpi.xyz
  spf: true
hosts:
- cert_expires: Sep 29 13:42:29 2026 GMT
  host: dagpi.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dagpi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dagpi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dagpi
provider_slug: dagpi
slug: dagpi-domain-security
source_filename: dagpi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dagpi.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:42:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dagpi.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dagpi/refs/heads/main/security/dagpi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Photography
- Public APIs
---
