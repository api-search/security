---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: twindo.com
  spf: true
hosts:
- cert_expires: Aug 30 00:34:13 2026 GMT
  host: www.twindo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Twindo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twindo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Twindo
provider_slug: twindo
slug: twindo-domain-security
source_filename: twindo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.twindo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 00:34:13 2026 GMT\n  hsts: false\ndomains:\n- domain: twindo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twindo/refs/heads/main/security/twindo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Spatial Intelligence
- LiDAR
- Scan to CAD
- BIM
- Digital Twins
- Reality Capture
- Architecture
- Construction
- Interior Design
---
