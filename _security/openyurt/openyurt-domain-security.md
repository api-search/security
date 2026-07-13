---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openyurt.io
  spf: false
hosts:
- cert_expires: Sep 28 05:18:24 2026 GMT
  host: openyurt.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openyurt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenYurt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenYurt
provider_slug: openyurt
slug: openyurt-domain-security
source_filename: openyurt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openyurt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:18:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: openyurt.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openyurt/refs/heads/main/security/openyurt-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Cloud-Edge
- Edge Computing
- Incubating
- IoT
- Kubernetes
---
