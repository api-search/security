---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jeh.aero
  spf: true
hosts:
- cert_expires: Aug 31 02:36:14 2026 GMT
  host: jeh.aero
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jeh Aerospace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jeh Aerospace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jeh Aerospace
provider_slug: jeh-aerospace
slug: jeh-aerospace-domain-security
source_filename: jeh-aerospace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jeh.aero\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 02:36:14 2026 GMT\n  hsts: false\ndomains:\n- domain: jeh.aero\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jeh-aerospace/refs/heads/main/security/jeh-aerospace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aerospace
- Manufacturing
- Aerostructures
- Aero-Engine Components
- Supply Chain
- Precision Machining
- India
---
