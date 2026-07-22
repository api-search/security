---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: enough-food.com
  spf: true
hosts:
- cert_expires: Sep 26 06:27:13 2026 GMT
  host: www.enough-food.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enough Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enough, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Enough
provider_slug: enough
slug: enough-domain-security
source_filename: enough-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enough-food.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 06:27:13 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: enough-food.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enough/refs/heads/main/security/enough-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food Technology
- Alternative Protein
- Sustainability
- Fermentation
- Mycoprotein
- AgTech
- Ingredients
---
