---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swingeducation.com
  spf: true
hosts:
- cert_expires: Sep 25 11:38:34 2026 GMT
  host: swingeducation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swing Education Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swing Education, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Swing Education
provider_slug: swing-education
slug: swing-education-domain-security
source_filename: swing-education-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swingeducation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 11:38:34 2026 GMT\n  hsts: false\ndomains:\n- domain: swingeducation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swing-education/refs/heads/main/security/swing-education-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- EdTech
- Staffing
- Substitute Teachers
- K-12
- Marketplace
- Workforce
---
