---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: watsco.com
  spf: true
hosts:
- cert_expires: Oct  3 04:00:40 2026 GMT
  host: www.watsco.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Watsco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Watsco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Watsco
provider_slug: watsco
slug: watsco-domain-security
source_filename: watsco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.watsco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 04:00:40 2026 GMT\n  hsts: false\ndomains:\n- domain: watsco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/watsco/refs/heads/main/security/watsco-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- HVAC
- Distribution
- B2B
- E-Commerce
- Refrigeration
- Fortune 1000
---
