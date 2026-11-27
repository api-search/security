---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ghurt.org
  spf: false
hosts:
- cert_expires: Jan 27 08:09:42 2027 GMT
  host: ghurt.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ghurt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ghurt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: ghurt
provider_slug: ghurt-org
slug: ghurt-org-domain-security
source_filename: ghurt-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ghurt.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 08:09:42 2027 GMT\n  hsts: false\ndomains:\n- domain: ghurt.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ghurt-org/security/ghurt-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Health
- Artificial Intelligence
- Data
- Personal-Analytics
- Free Tier
- Open Source
---
