---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pinnaclewest.com
  spf: true
hosts:
- cert_expires: Sep 10 03:24:43 2026 GMT
  host: www.pinnaclewest.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinnacle West Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pinnacle-west-capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: pinnacle-west-capital
provider_slug: pinnacle-west-capital
slug: pinnacle-west-capital-domain-security
source_filename: pinnacle-west-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pinnaclewest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 03:24:43 2026 GMT\n  hsts: false\ndomains:\n- domain: pinnaclewest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinnacle-west-capital/refs/heads/main/security/pinnacle-west-capital-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 1000
---
