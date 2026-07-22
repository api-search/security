---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: roon.com
  spf: true
hosts:
- cert_expires: Sep  2 06:58:29 2026 GMT
  host: www.roon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Roon
provider_slug: roon
slug: roon-domain-security
source_filename: roon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.roon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 06:58:29 2026 GMT\n  hsts: null\ndomains:\n- domain: roon.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roon/refs/heads/main/security/roon-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Health
- Digital Health
- Health Information
- Patient Education
- Telehealth
- Medical Experts
- Consumer Health
---
