---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: studio-moderna.com
  spf: true
hosts:
- cert_expires: Aug 21 21:01:59 2026 GMT
  host: www.studio-moderna.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Studio Moderna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Studio Moderna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Studio Moderna
provider_slug: studio-moderna
slug: studio-moderna-domain-security
source_filename: studio-moderna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.studio-moderna.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 21 21:01:59 2026 GMT\n  hsts: false\ndomains:\n- domain: studio-moderna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/studio-moderna/refs/heads/main/security/studio-moderna-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Retail
- E-commerce
- Consumer Goods
- Direct-to-Consumer
- Multichannel Retail
- Central and Eastern Europe
---
