---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: science37.com
  spf: true
hosts:
- cert_expires: Sep 14 05:38:43 2026 GMT
  host: science37.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Science 37 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Science 37 *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Science 37 *
provider_slug: science-37
slug: science-37-domain-security
source_filename: science-37-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: science37.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:38:43 2026 GMT\n  hsts: false\ndomains:\n- domain: science37.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/science-37/refs/heads/main/security/science-37-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Clinical Trials
- Clinical Research
- Decentralized Clinical Trials
- Healthcare
- Patient Recruitment
- Telemedicine
---
