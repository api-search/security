---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sdge.com
  spf: true
hosts:
- cert_expires: Apr  9 23:59:59 2027 GMT
  host: www.sdge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sdge Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for San Diego Gas & Electric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: San Diego Gas & Electric
provider_slug: sdge-com
slug: sdge-com-domain-security
source_filename: sdge-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sdge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sdge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sdge-com/refs/heads/main/security/sdge-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Utilities
- Electricity
- Natural Gas
- Green Button
- Energy Data
---
