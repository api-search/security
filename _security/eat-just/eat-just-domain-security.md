---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ju.st
  spf: true
hosts:
- cert_expires: Oct 23 11:40:02 2026 GMT
  host: www.ju.st
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eat Just Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eat Just, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eat Just
provider_slug: eat-just
slug: eat-just-domain-security
source_filename: eat-just-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ju.st\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 11:40:02 2026 GMT\n  hsts: null\ndomains:\n- domain: ju.st\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eat-just/refs/heads/main/security/eat-just-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food
- Food and Beverage
- Consumer Packaged Goods
- Plant-Based
- Alternative Protein
- Cultivated Meat
- Food Technology
- Agriculture
- Manufacturing
---
