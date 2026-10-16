---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cellphire.com
  spf: true
hosts:
- cert_expires: Nov 28 11:12:30 2026 GMT
  host: www.cellphire.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cellphire Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CellPhire Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CellPhire Therapeutics
provider_slug: cellphire-therapeutics
slug: cellphire-therapeutics-domain-security
source_filename: cellphire-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cellphire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 11:12:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cellphire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellphire-therapeutics/refs/heads/main/security/cellphire-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Therapeutics
- Platelet
- Hemostasis
---
