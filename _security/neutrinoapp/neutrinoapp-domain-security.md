---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: neutrinoapp.com
  spf: true
hosts:
- cert_expires: Dec 26 20:00:44 2026 GMT
  host: neutrinoapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Neutrinoapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neutrino AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Neutrino AI
provider_slug: neutrinoapp
slug: neutrinoapp-domain-security
source_filename: neutrinoapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neutrinoapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 20:00:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: neutrinoapp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/neutrinoapp/security/neutrinoapp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Machine Learning
- Data Analytics
- Enterprise
- Platform
- Company
---
