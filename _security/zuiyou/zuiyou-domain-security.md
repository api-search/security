---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: izuiyou.com
  spf: false
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: www.izuiyou.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zuiyou Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zuiyou, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Zuiyou
provider_slug: zuiyou
slug: zuiyou-domain-security
source_filename: zuiyou-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.izuiyou.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: izuiyou.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/zuiyou/security/zuiyou-domain-security.yml
summary_line: TLSv1.2
tags:
- Social
- Community
- Mobile
- Entertainment
- China
---
