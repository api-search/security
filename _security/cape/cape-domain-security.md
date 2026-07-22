---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cape.co
  spf: true
hosts:
- cert_expires: Aug 18 04:01:21 2026 GMT
  host: www.cape.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cape, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cape
provider_slug: cape
slug: cape-domain-security
source_filename: cape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cape.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 04:01:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cape.co\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cape/refs/heads/main/security/cape-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Privacy
- Mobile
- Telecommunications
- Carrier
- MVNO
- Security
- Consumer
---
