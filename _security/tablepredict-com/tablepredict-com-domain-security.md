---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: true
  domain: tablepredict.com
  spf: true
hosts:
- cert_expires: Jan  1 08:27:11 2027 GMT
  host: tablepredict.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TablePredict Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TablePredict, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: TablePredict
provider_slug: tablepredict-com
slug: tablepredict-com-domain-security
source_filename: tablepredict-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tablepredict.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 08:27:11 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tablepredict.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tablepredict-com/security/tablepredict-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Prediction Games
- Leaderboard
- Community
---
