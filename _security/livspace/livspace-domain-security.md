---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: livspace.com
  spf: true
hosts:
- cert_expires: Aug 27 19:40:38 2026 GMT
  host: www.livspace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Livspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Livspace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Livspace
provider_slug: livspace
slug: livspace-domain-security
source_filename: livspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.livspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:40:38 2026 GMT\n  hsts: false\ndomains:\n- domain: livspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/livspace/refs/heads/main/security/livspace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Interior Design
- Home Renovation
- Home Improvement
- Modular Kitchens
- Home Services
- India
- E-commerce
---
