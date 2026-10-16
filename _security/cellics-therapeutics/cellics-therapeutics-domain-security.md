---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cellics.com
  spf: true
hosts:
- cert_expires: Nov 30 13:02:45 2026 GMT
  host: www.cellics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cellics Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cellics Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cellics Therapeutics
provider_slug: cellics-therapeutics
slug: cellics-therapeutics-domain-security
source_filename: cellics-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cellics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 13:02:45 2026 GMT\n  hsts: false\ndomains:\n- domain: cellics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellics-therapeutics/refs/heads/main/security/cellics-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Therapeutics
- Inflammation
- Immunology
---
