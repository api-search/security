---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: httpstatus.com
  spf: false
hosts:
- cert_expires: Dec  3 17:46:22 2026 GMT
  host: httpstatus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Httpstatus Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for httpstatus-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: httpstatus-com
provider_slug: httpstatus-com
slug: httpstatus-com-domain-security
source_filename: httpstatus-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: httpstatus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 17:46:22 2026 GMT\n  hsts: false\ndomains:\n- domain: httpstatus.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/httpstatus-com/security/httpstatus-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- HTTP
- StatusCodes
- DeveloperTools
- API
- OpenSource
---
