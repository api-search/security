---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pheontx.com
  spf: true
hosts:
- cert_expires: Aug 25 19:51:40 2026 GMT
  host: pheontx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pheon Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pheon Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pheon Therapeutics
provider_slug: pheon-therapeutics
slug: pheon-therapeutics-domain-security
source_filename: pheon-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pheontx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 19:51:40 2026 GMT\n  hsts: false\ndomains:\n- domain: pheontx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pheon-therapeutics/refs/heads/main/security/pheon-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Antibody-Drug Conjugates
- Drug Development
- Healthcare
- Cancer Therapeutics
---
