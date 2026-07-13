---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: judge0.com
  spf: true
hosts:
- cert_expires: Sep  3 15:16:01 2026 GMT
  host: ce.judge0.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Judge0 Ce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Judge0 CE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Judge0 CE
provider_slug: judge0-ce
slug: judge0-ce-domain-security
source_filename: judge0-ce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ce.judge0.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 15:16:01 2026 GMT\n  hsts: false\ndomains:\n- domain: judge0.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/judge0-ce/refs/heads/main/security/judge0-ce-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Programming
- Public APIs
---
