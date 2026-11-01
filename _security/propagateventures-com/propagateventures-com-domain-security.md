---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: propagateventures.com
  spf: true
hosts:
- cert_expires: Dec  7 16:13:19 2026 GMT
  host: propagateventures.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Propagateventures Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Propagate Ventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Propagate Ventures
provider_slug: propagateventures-com
slug: propagateventures-com-domain-security
source_filename: propagateventures-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: propagateventures.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 16:13:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: propagateventures.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/propagateventures-com/security/propagateventures-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Venture
- Techstars
- Startup
- Portfolio
---
