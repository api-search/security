---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: impossiblefoods.com
  spf: false
hosts:
- cert_expires: Sep 17 12:46:16 2026 GMT
  host: impossiblefoods.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Impossible Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Impossible Foods, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Impossible Foods
provider_slug: impossible-foods
slug: impossible-foods-domain-security
source_filename: impossible-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: impossiblefoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 12:46:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: impossiblefoods.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impossible-foods/refs/heads/main/security/impossible-foods-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Frontier Tech
- Food
- Food Technology
- Plant-Based
- Alternative Protein
- Consumer Packaged Goods
- Sustainability
---
