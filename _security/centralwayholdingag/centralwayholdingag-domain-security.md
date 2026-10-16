---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: centralwaygroup.com
  spf: true
hosts:
- cert_expires: Nov 10 21:51:25 2026 GMT
  host: centralwaygroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Centralwayholdingag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centralwayholdingag, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Centralwayholdingag
provider_slug: centralwayholdingag
slug: centralwayholdingag-domain-security
source_filename: centralwayholdingag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: centralwaygroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 21:51:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: centralwaygroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centralwayholdingag/refs/heads/main/security/centralwayholdingag-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Holding
- Investment
- Swiss
- Finance
---
