---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: faircraft.bio
  spf: true
hosts:
- cert_expires: Aug  9 10:12:38 2026 GMT
  host: faircraft.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Faircraft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Faircraft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Faircraft
provider_slug: faircraft
slug: faircraft-domain-security
source_filename: faircraft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: faircraft.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 10:12:38 2026 GMT\n  hsts: false\ndomains:\n- domain: faircraft.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/faircraft/refs/heads/main/security/faircraft-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Cultivated Leather
- Advanced Materials
- Sustainability
- Manufacturing
---
