---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thrivefantasy.com
  spf: true
hosts:
- cert_expires: Oct  9 17:45:22 2026 GMT
  host: www.thrivefantasy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thrivefantasy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThriveFantasy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ThriveFantasy
provider_slug: thrivefantasy
slug: thrivefantasy-domain-security
source_filename: thrivefantasy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thrivefantasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 17:45:22 2026 GMT\n  hsts: false\ndomains:\n- domain: thrivefantasy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thrivefantasy/refs/heads/main/security/thrivefantasy-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fantasy Sports
- Sports
- Gaming
- Player Props
- Contests
- Defunct
---
