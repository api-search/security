---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tedivirtual.com
  spf: true
hosts:
- cert_expires: Sep  6 09:22:43 2026 GMT
  host: tedivirtual.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tedi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TEDI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TEDI
provider_slug: tedi
slug: tedi-domain-security
source_filename: tedi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tedivirtual.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 09:22:43 2026 GMT\n  hsts: false\ndomains:\n- domain: tedivirtual.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tedi/refs/heads/main/security/tedi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- EdTech
- Construction
- Engineering
- Professional Training
- Certification
- Latin America
---
