---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: user1st.com
  spf: true
hosts:
- cert_expires: Oct  3 04:09:56 2026 GMT
  host: user1st.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: User1St Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for User1st, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: User1st
provider_slug: user1st
slug: user1st-domain-security
source_filename: user1st-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: user1st.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 04:09:56 2026 GMT\n  hsts: false\ndomains:\n- domain: user1st.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/user1st/refs/heads/main/security/user1st-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Accessibility
- Digital Accessibility
- WCAG
- ADA
- EAA Compliance
- Web Accessibility
- Mobile Accessibility
- Compliance
---
