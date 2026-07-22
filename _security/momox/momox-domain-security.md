---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: momox.de
  spf: true
hosts:
- cert_expires: Sep 30 14:09:53 2026 GMT
  host: www.momox.de
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Momox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Momox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Momox
provider_slug: momox
slug: momox-domain-security
source_filename: momox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.momox.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:09:53 2026 GMT\n  hsts: null\ndomains:\n- domain: momox.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/momox/refs/heads/main/security/momox-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Re-Commerce
- Marketplace
- Second-Hand
- Books
- Media
- Fashion
- E-Commerce
- Sustainability
- Germany
---
