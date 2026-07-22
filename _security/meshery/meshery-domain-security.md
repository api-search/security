---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meshery.io
  spf: false
hosts:
- cert_expires: Sep 25 00:54:18 2026 GMT
  host: meshery.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meshery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meshery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Meshery
provider_slug: meshery
slug: meshery-domain-security
source_filename: meshery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meshery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 00:54:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: meshery.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meshery/refs/heads/main/security/meshery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Native
- CNCF
- Kubernetes
- Service Mesh
- Platform Engineering
- Multi-Cluster
---
