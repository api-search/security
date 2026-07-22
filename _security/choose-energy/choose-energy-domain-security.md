---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chooseenergy.com
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: www.chooseenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Choose Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Choose Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Choose Energy
provider_slug: choose-energy
slug: choose-energy-domain-security
source_filename: choose-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chooseenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: chooseenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/choose-energy/refs/heads/main/security/choose-energy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Energy
- Electricity
- Natural Gas
- Marketplace
- Utilities
- Comparison
- Deregulated Energy
- Solar
---
