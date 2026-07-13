---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: apicagent.com
  spf: false
hosts:
- cert_expires: Sep 17 11:03:52 2026 GMT
  host: www.apicagent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apicagent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ApicAgent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: ApicAgent
provider_slug: apicagent
slug: apicagent-domain-security
source_filename: apicagent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apicagent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 11:03:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apicagent.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicagent/refs/heads/main/security/apicagent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Development
- Public APIs
---
