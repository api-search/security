---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: amogy.co
  spf: true
hosts:
- cert_expires: Sep 22 19:39:55 2026 GMT
  host: amogy.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amogy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amogy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Amogy
provider_slug: amogy
slug: amogy-domain-security
source_filename: amogy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amogy.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 19:39:55 2026 GMT\n  hsts: false\ndomains:\n- domain: amogy.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amogy/refs/heads/main/security/amogy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Energy
- Clean Energy
- Ammonia
- Decarbonization
- Hydrogen
- Power Generation
- Maritime
- Sustainability
---
