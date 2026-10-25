---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pls.com
  spf: true
hosts:
- cert_expires: Dec 15 02:57:32 2026 GMT
  host: pls.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pls Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PLS Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PLS Group
provider_slug: pls-group
slug: pls-group-domain-security
source_filename: pls-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pls.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 02:57:32 2026 GMT\n  hsts: null\ndomains:\n- domain: pls.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pls-group/refs/heads/main/security/pls-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Lithium
- Mining
- Battery Materials
- Australia
- ASX Listed
---
