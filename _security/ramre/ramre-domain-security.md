---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aoreltd.com
  spf: true
hosts:
- cert_expires: Aug 29 23:59:04 2026 GMT
  host: aoreltd.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ramre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ramre, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ramre
provider_slug: ramre
slug: ramre-domain-security
source_filename: ramre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aoreltd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:59:04 2026 GMT\n  hsts: false\ndomains:\n- domain: aoreltd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ramre/refs/heads/main/security/ramre-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- Reinsurance
- Financial Services
- Auto Insurance
- Bermuda
---
