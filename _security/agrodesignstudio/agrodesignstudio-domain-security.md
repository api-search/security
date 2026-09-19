---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agrodesign.co.jp
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: agrobox.jp
  spf: true
hosts:
- cert_expires: Oct 23 00:22:35 2026 GMT
  host: www.agrodesign.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  3 06:50:46 2026 GMT
  host: www.agrobox.jp
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 03:48:34 2026 GMT
  host: www.agrodesign.shop
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Agrodesignstudio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgroDesign Studios, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AgroDesign Studios
provider_slug: agrodesignstudio
slug: agrodesignstudio-domain-security
source_filename: agrodesignstudio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agrodesign.co.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 00:22:35 2026 GMT\n  hsts: false\n- host: www.agrobox.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 06:50:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: www.agrodesign.shop\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 03:48:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: agrodesign.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: agrobox.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrodesignstudio/refs/heads/main/security/agrodesignstudio-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Agriculture
- AgTech
- Biotechnology
- Life Sciences
- Structural Biology
- Drug Discovery
- Crop Protection
- Contract Research
- Laboratory Automation
- Japan
- MCP
- Company
---
