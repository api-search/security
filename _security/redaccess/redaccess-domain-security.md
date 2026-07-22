---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: redaccess.io
  spf: true
hosts:
- cert_expires: Sep 29 04:59:21 2026 GMT
  host: redaccess.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redaccess Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red Access, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Red Access
provider_slug: redaccess
slug: redaccess-domain-security
source_filename: redaccess-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redaccess.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:59:21 2026 GMT\n  hsts: false\ndomains:\n- domain: redaccess.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redaccess/refs/heads/main/security/redaccess-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Cybersecurity
- Secure Service Edge
- Browser Security
- Zero Trust
- Data Loss Prevention
- SSE
---
