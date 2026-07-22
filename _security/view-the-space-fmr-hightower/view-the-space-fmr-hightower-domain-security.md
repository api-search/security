---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vts.com
  spf: true
hosts:
- cert_expires: Sep  5 16:46:23 2026 GMT
  host: www.vts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: View The Space Fmr Hightower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for View The Space (Fmr Hightower), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: View The Space (Fmr Hightower)
provider_slug: view-the-space-fmr-hightower
slug: view-the-space-fmr-hightower-domain-security
source_filename: view-the-space-fmr-hightower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 16:46:23 2026 GMT\n  hsts: null\ndomains:\n- domain: vts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/view-the-space-fmr-hightower/refs/heads/main/security/view-the-space-fmr-hightower-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Vertical Software
- Commercial Real Estate
- Real Estate
- PropTech
- Leasing
- Asset Management
- SaaS
---
