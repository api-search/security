---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: polopan.com
  spf: true
hosts:
- cert_expires: Dec 13 16:16:04 2026 GMT
  host: polopan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Polopan Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for polopan-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: polopan-com
provider_slug: polopan-com
slug: polopan-com-domain-security
source_filename: polopan-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polopan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 16:16:04 2026 GMT\n  hsts: false\ndomains:\n- domain: polopan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/polopan-com/security/polopan-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Fashion
- PersonalStylist
- E-commerce
---
