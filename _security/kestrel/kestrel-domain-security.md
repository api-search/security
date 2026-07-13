---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: usekestrel.ai
  spf: false
hosts:
- cert_expires: Sep 21 14:46:00 2026 GMT
  host: usekestrel.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 14:46:00 2026 GMT
  host: docs.usekestrel.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kestrel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kestrel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kestrel
provider_slug: kestrel
slug: kestrel-domain-security
source_filename: kestrel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usekestrel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:46:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.usekestrel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:46:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: usekestrel.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kestrel/refs/heads/main/security/kestrel-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Agents
- Cloud Security
- Incident Response
- Kubernetes
- Observability
---
