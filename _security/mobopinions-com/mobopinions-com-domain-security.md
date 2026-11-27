---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mobopinions.com
  spf: true
hosts:
- cert_expires: Dec 26 01:38:09 2026 GMT
  host: mobopinions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MOBOPINIONS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MOBOPINIONS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MOBOPINIONS
provider_slug: mobopinions-com
slug: mobopinions-com-domain-security
source_filename: mobopinions-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mobopinions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 01:38:09 2026 GMT\n  hsts: false\ndomains:\n- domain: mobopinions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mobopinions-com/security/mobopinions-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Market Research
- Mobile
- Artificial Intelligence
- Surveys
- Global
---
