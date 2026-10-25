---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: brambles.com
  spf: true
hosts:
- cert_expires: Dec 31 19:57:18 2026 GMT
  host: brambles.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brambles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brambles, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Brambles
provider_slug: brambles
slug: brambles-domain-security
source_filename: brambles-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brambles.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 19:57:18 2026 GMT\n  hsts: false\ndomains:\n- domain: brambles.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brambles/refs/heads/main/security/brambles-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Logistics
- Supply Chain
- Pallet Pooling
- Reusable Packaging
- Sustainability
- Australia
---
