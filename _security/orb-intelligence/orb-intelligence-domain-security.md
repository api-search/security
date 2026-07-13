---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orb-intelligence.com
  spf: false
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: api.orb-intelligence.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orb Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ORB Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ORB Intelligence
provider_slug: orb-intelligence
slug: orb-intelligence-domain-security
source_filename: orb-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.orb-intelligence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: orb-intelligence.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orb-intelligence/refs/heads/main/security/orb-intelligence-domain-security.yml
summary_line: TLSv1.3
tags:
- Business
- Public APIs
---
