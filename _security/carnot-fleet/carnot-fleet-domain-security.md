---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carnotfleet.com
  spf: true
hosts:
- cert_expires: Nov 18 11:37:14 2026 GMT
  host: carnotfleet.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Carnot Fleet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carnot Fleet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Carnot Fleet
provider_slug: carnot-fleet
slug: carnot-fleet-domain-security
source_filename: carnot-fleet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carnotfleet.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 18 11:37:14 2026 GMT\n  hsts: false\ndomains:\n- domain: carnotfleet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carnot-fleet/refs/heads/main/security/carnot-fleet-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Cold Chain
- Logistics
- Supply Chain
- Refrigeration
- Temperature Monitoring
- IoT
- Fleet
- Hardware
---
