---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cambiumglobal.com
  spf: true
hosts:
- cert_expires: Oct  2 00:48:38 2026 GMT
  host: cambiumglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cambium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cambium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cambium
provider_slug: cambium
slug: cambium-domain-security
source_filename: cambium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cambiumglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 00:48:38 2026 GMT\n  hsts: false\ndomains:\n- domain: cambiumglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cambium/refs/heads/main/security/cambium-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Advanced Materials
- Materials Science
- Defense
- Aerospace
- Composites
- Manufacturing
---
