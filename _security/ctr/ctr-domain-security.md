---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ctr.co.kr
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: www.ctr.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ctr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CTR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CTR
provider_slug: ctr
slug: ctr-domain-security
source_filename: ctr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ctr.co.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ctr.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ctr/refs/heads/main/security/ctr-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Mobility
- Safety
- Innovation
- ESG
---
