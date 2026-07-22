---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: visuallogix.com
  spf: true
hosts:
- cert_expires: Oct 19 10:54:16 2026 GMT
  host: visuallogix.com
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Visuallogix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VisualLogix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: VisualLogix
provider_slug: visuallogix
slug: visuallogix-domain-security
source_filename: visuallogix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: visuallogix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 10:54:16 2026 GMT\n  hsts: true\n  hsts_max_age: 2628000\ndomains:\n- domain: visuallogix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visuallogix/refs/heads/main/security/visuallogix-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- CAD
- Computer-Aided Design
- Simulation
- Engineering Software
- Analytics
- Modeling
---
