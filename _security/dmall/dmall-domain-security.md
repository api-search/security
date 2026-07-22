---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dmall.com
  spf: true
hosts:
- cert_expires: Dec 12 03:58:32 2026 GMT
  host: www.dmall.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dmall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DMall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DMall
provider_slug: dmall
slug: dmall-domain-security
source_filename: dmall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dmall.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 03:58:32 2026 GMT\n  hsts: false\ndomains:\n- domain: dmall.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dmall/refs/heads/main/security/dmall-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Consumer
- Retail
- E-Commerce
- SaaS
- Digital Retail
- Supply Chain
- China
---
