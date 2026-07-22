---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: acadium.com
  spf: true
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: acadium.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GenM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GenM
provider_slug: genm
slug: genm-domain-security
source_filename: genm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acadium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: acadium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genm/refs/heads/main/security/genm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Digital Marketing
- Education
- Apprenticeships
- Marketing Talent
- Online Courses
- Career Platform
- Mentorship
---
