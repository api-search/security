---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fluidvip.com
  spf: true
hosts:
- cert_expires: Jan  5 01:54:46 2027 GMT
  host: fluidvip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fluid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fluid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fluid
provider_slug: fluidvip-com
slug: fluidvip-com-domain-security
source_filename: fluidvip-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fluidvip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 01:54:46 2027 GMT\n  hsts: false\ndomains:\n- domain: fluidvip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fluidvip-com/security/fluidvip-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Software-as-a-Service
- Content Generation
- Automation
- Marketing
---
