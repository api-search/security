---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: welltrack.com
  spf: true
hosts:
- cert_expires: Aug 28 23:59:59 2026 GMT
  host: welltrack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cyberpsyc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cyberpsyc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cyberpsyc
provider_slug: cyberpsyc
slug: cyberpsyc-domain-security
source_filename: cyberpsyc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: welltrack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: welltrack.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyberpsyc/refs/heads/main/security/cyberpsyc-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Mental Health
- Behavioral Health
- Wellness
- Digital Therapeutics
- CBT
- Healthcare
- Higher Education
- SSO
---
