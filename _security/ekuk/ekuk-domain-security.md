---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ohuseire.ee
  spf: false
hosts:
- cert_expires: Dec 25 15:50:13 2026 GMT
  host: ohuseire.ee
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ekuk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EKUK (Estonia), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: EKUK (Estonia)
provider_slug: ekuk
slug: ekuk-domain-security
source_filename: ekuk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ohuseire.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 15:50:13 2026 GMT\n  hsts: false\ndomains:\n- domain: ohuseire.ee\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ekuk/security/ekuk-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Estonia
- Technology
- Corporate
- WebPresence
---
