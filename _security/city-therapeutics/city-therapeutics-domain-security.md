---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: citytx.com
  spf: true
hosts:
- cert_expires: Sep 18 14:27:43 2026 GMT
  host: www.citytx.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: City Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: City Therapeutics
provider_slug: city-therapeutics
slug: city-therapeutics-domain-security
source_filename: city-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.citytx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:27:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: citytx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/city-therapeutics/refs/heads/main/security/city-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Therapeutics
- RNAi
- Drug Discovery
- Clinical Stage
- Genetic Medicine
---
