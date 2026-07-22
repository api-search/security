---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: plena.health
  spf: true
hosts:
- cert_expires: Sep 21 03:56:32 2026 GMT
  host: www.plena.health
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plena Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plena Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Plena Health
provider_slug: plena-health
slug: plena-health-domain-security
source_filename: plena-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plena.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:56:32 2026 GMT\n  hsts: false\ndomains:\n- domain: plena.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plena-health/refs/heads/main/security/plena-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Healthcare
- Medical Practice
- Artificial Intelligence
- Automation
- Workflow
- Y Combinator
---
