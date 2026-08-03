---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carbyne.com
  spf: true
hosts:
- cert_expires: Sep 27 13:30:58 2026 GMT
  host: carbyne.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carbyne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carbyne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Carbyne
provider_slug: carbyne
slug: carbyne-domain-security
source_filename: carbyne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carbyne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 13:30:58 2026 GMT\n  hsts: false\ndomains:\n- domain: carbyne.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbyne/refs/heads/main/security/carbyne-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Emergency Services
- Public Safety
- Communications
- Telecommunications
- NG911
- Contact Center
- Location
- Video
- Government
- Artificial Intelligence
---
