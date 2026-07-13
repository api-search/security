---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dredd.org
  spf: false
hosts:
- cert_expires: Oct  3 20:30:06 2026 GMT
  host: dredd.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dredd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dredd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dredd
provider_slug: dredd
slug: dredd-domain-security
source_filename: dredd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dredd.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:30:06 2026 GMT\n  hsts: false\ndomains:\n- domain: dredd.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dredd/refs/heads/main/security/dredd-domain-security.yml
summary_line: TLSv1.3
tags:
- Contract Testing
- API Testing
- OpenAPI
- API Blueprint
- Tooling
---
