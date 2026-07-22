---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ubras.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ubras.cn
  spf: false
hosts:
- cert_expires: Sep  1 14:01:32 2026 GMT
  host: ubras.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 04:31:46 2026 GMT
  host: www.ubras.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ubras Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ubras, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ubras
provider_slug: ubras
slug: ubras-domain-security
source_filename: ubras-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ubras.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 14:01:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: www.ubras.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 04:31:46 2026 GMT\n  hsts: false\ndomains:\n- domain: ubras.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: ubras.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubras/refs/heads/main/security/ubras-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Retail
- eCommerce
- Apparel
- Intimate Apparel
- Direct-to-Consumer
- Agentic Commerce
---
