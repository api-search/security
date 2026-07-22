---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vetsource.com
  spf: true
hosts:
- cert_expires: Sep 15 14:41:47 2026 GMT
  host: vetsource.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vetsource Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VetSource, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VetSource
provider_slug: vetsource
slug: vetsource-domain-security
source_filename: vetsource-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vetsource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:41:47 2026 GMT\n  hsts: false\ndomains:\n- domain: vetsource.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vetsource/refs/heads/main/security/vetsource-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Veterinary
- Pharmacy
- Pet Health
- Practice Management
- Client Engagement
- Data Analytics
---
