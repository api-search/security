---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hammerspace.com
  spf: true
hosts:
- cert_expires: Sep  6 21:55:12 2026 GMT
  host: hammerspace.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hammerspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hammerspace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hammerspace
provider_slug: hammerspace
slug: hammerspace-domain-security
source_filename: hammerspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hammerspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 21:55:12 2026 GMT\n  hsts: null\ndomains:\n- domain: hammerspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hammerspace/refs/heads/main/security/hammerspace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Storage
- Data Management
- Filesystem
- Data Orchestration
- Hybrid Cloud
- Kubernetes
- Artificial Intelligence
- Unstructured Data
- Infrastructure
---
