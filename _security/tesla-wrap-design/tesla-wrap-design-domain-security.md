---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tesla-wrap.design
  spf: true
hosts:
- cert_expires: Feb  7 12:26:57 2027 GMT
  host: tesla-wrap.design
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tesla Wrap Designer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tesla Wrap Designer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tesla Wrap Designer
provider_slug: tesla-wrap-design
slug: tesla-wrap-design-domain-security
source_filename: tesla-wrap-design-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tesla-wrap.design\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 12:26:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tesla-wrap.design\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tesla-wrap-design/security/tesla-wrap-design-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Vehicle Wrap Design
- 3D Preview
- AI Generator
- UV Templates
- Tesla Community
---
