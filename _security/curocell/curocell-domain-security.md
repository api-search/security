---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: curocellbtx.com
  spf: true
hosts:
- cert_expires: Nov 28 13:36:50 2026 GMT
  host: curocellbtx.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curocell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curocell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Curocell
provider_slug: curocell
slug: curocell-domain-security
source_filename: curocell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curocellbtx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 28 13:36:50 2026 GMT\n  hsts: false\ndomains:\n- domain: curocellbtx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curocell/refs/heads/main/security/curocell-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Biotechnology
- Cell Therapy
- Oncology
- CAR-T
---
