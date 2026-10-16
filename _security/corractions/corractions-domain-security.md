---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: corractions.com
  spf: false
hosts:
- cert_expires: Nov 28 10:11:57 2026 GMT
  host: corractions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Corractions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corractions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Corractions
provider_slug: corractions
slug: corractions-domain-security
source_filename: corractions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corractions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 10:11:57 2026 GMT\n  hsts: false\ndomains:\n- domain: corractions.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corractions/refs/heads/main/security/corractions-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI
- Automotive
- Safety
- Neurotechnology
---
