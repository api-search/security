---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: preveil.com
  spf: true
hosts:
- cert_expires: Oct 14 08:20:42 2026 GMT
  host: www.preveil.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Preveil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PreVeil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: PreVeil
provider_slug: preveil
slug: preveil-domain-security
source_filename: preveil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.preveil.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 08:20:42 2026 GMT\n  hsts: false\ndomains:\n- domain: preveil.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preveil/refs/heads/main/security/preveil-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Encryption
- End-to-End Encryption
- Email
- File Sharing
- Security
- Compliance
- CMMC
- ITAR
- CUI
- Defense
- Cybersecurity
- Data Protection
---
