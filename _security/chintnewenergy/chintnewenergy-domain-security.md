---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: chint.com
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: energy.chint.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chintnewenergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chintnewenergy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Chintnewenergy
provider_slug: chintnewenergy
slug: chintnewenergy-domain-security
source_filename: chintnewenergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: energy.chint.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: chint.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chintnewenergy/refs/heads/main/security/chintnewenergy-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Energy
- Solar
- CleanTech
- China
- Renewable
---
