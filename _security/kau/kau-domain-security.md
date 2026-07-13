---
description: ''
domains:
- caa:
  - 0 issue "Digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kau.edu.sa
  spf: true
hosts:
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: www.kau.edu.sa
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kau Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for King Abdulaziz University, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: King Abdulaziz University
provider_slug: kau
slug: kau-domain-security
source_filename: kau-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kau.edu.sa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kau.edu.sa\n  dnssec: true\n  caa:\n  - 0 issue \"Digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kau/refs/heads/main/security/kau-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Saudi Arabia
- Middle East
---
