---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ouroborosapps.com
  spf: false
hosts:
- cert_expires: Jan  2 21:36:33 2027 GMT
  host: ouroborosapps.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ouroboros Apps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ouroboros Apps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Ouroboros Apps
provider_slug: ouroborosapps-com
slug: ouroborosapps-com-domain-security
source_filename: ouroborosapps-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ouroborosapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 21:36:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ouroborosapps.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ouroborosapps-com/security/ouroborosapps-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Plugins
- Automation
- Productivity
- ChatGPT
---
