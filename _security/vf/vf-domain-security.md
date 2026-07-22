---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vfc.com
  spf: true
hosts:
- cert_expires: Sep 22 08:02:45 2026 GMT
  host: www.vfc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VF Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VF Corporation
provider_slug: vf
slug: vf-domain-security
source_filename: vf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vfc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 08:02:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vfc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vf/refs/heads/main/security/vf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apparel
- Fashion
- Retail
- E-Commerce
- Footwear
- Fortune 500
---
