---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gymshark.com
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: www.gymshark.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 20:07:13 2026 GMT
  host: auth.gymshark.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gymshark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gymshark, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gymshark
provider_slug: gymshark
slug: gymshark-domain-security
source_filename: gymshark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gymshark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\n- host: auth.gymshark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 20:07:13 2026 GMT\n  hsts: null\ndomains:\n- domain: gymshark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gymshark/refs/heads/main/security/gymshark-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Fitness
- Consumer
- Direct To Consumer
- Identity
- OpenID Connect
---
