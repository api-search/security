---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dcndx.com
  spf: true
hosts:
- cert_expires: Dec 13 07:02:22 2026 GMT
  host: dcndx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chinadiagnosticmedicalcorporationcdmc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chinadiagnosticmedicalcorporationcdmc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chinadiagnosticmedicalcorporationcdmc
provider_slug: chinadiagnosticmedicalcorporationcdmc
slug: chinadiagnosticmedicalcorporationcdmc-domain-security
source_filename: chinadiagnosticmedicalcorporationcdmc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dcndx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 07:02:22 2026 GMT\n  hsts: false\ndomains:\n- domain: dcndx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chinadiagnosticmedicalcorporationcdmc/refs/heads/main/security/chinadiagnosticmedicalcorporationcdmc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- IVD
- CDMO
- CRO
- Diagnostics
- California
---
