---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cheapcadtools.com
  spf: true
hosts:
- cert_expires: Dec 26 20:41:08 2026 GMT
  host: cheapcadtools.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cheapcadtools Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CheapCADTools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CheapCADTools
provider_slug: cheapcadtools-com
slug: cheapcadtools-com-domain-security
source_filename: cheapcadtools-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cheapcadtools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 20:41:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cheapcadtools.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cheapcadtools-com/security/cheapcadtools-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CAD
- Engineering
- Tools
- Manufacturing
- Open Source
---
