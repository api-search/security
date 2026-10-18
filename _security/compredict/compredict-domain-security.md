---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: compredict.ai
  spf: true
hosts:
- cert_expires: Dec  2 10:07:04 2026 GMT
  host: compredict.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Compredict Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Compredict, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Compredict
provider_slug: compredict
slug: compredict-domain-security
source_filename: compredict-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compredict.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 10:07:04 2026 GMT\n  hsts: false\ndomains:\n- domain: compredict.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/compredict/refs/heads/main/security/compredict-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Artificial Intelligence
- Automotive
- Sensors
- Virtual
---
