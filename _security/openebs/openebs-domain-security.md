---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openebs.io
  spf: true
hosts:
- cert_expires: Sep  1 16:28:58 2026 GMT
  host: openebs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openebs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenEBS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenEBS
provider_slug: openebs
slug: openebs-domain-security
source_filename: openebs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openebs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 16:28:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openebs.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openebs/refs/heads/main/security/openebs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Containers
- Kubernetes
- Open Source
- Persistent Storage
- Storage
---
