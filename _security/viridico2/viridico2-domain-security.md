---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: viridico2.co.uk
  spf: true
hosts:
- cert_expires: Oct 19 22:52:26 2026 GMT
  host: viridico2.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Viridico2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ViridiCO2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: ViridiCO2
provider_slug: viridico2
slug: viridico2-domain-security
source_filename: viridico2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: viridico2.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 22:52:26 2026 GMT\n  hsts: false\ndomains:\n- domain: viridico2.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viridico2/refs/heads/main/security/viridico2-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sustainability
- Carbon Capture
- Carbon Utilization
- Green Chemistry
- Climate
- CO2
---
