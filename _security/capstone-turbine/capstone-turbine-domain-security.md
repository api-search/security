---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: capstoneenergyplus.com
  spf: true
hosts:
- cert_expires: Oct 12 08:01:53 2026 GMT
  host: www.capstoneenergyplus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capstone Turbine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capstone Turbine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Capstone Turbine
provider_slug: capstone-turbine
slug: capstone-turbine-domain-security
source_filename: capstone-turbine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.capstoneenergyplus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 08:01:53 2026 GMT\n  hsts: false\ndomains:\n- domain: capstoneenergyplus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capstone-turbine/refs/heads/main/security/capstone-turbine-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Microturbines
- Clean Energy
- Power Generation
- Microgrid
- Combined Heat and Power
- Manufacturing
---
