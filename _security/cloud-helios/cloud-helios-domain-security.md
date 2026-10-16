---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: helios.id
  spf: true
hosts:
- cert_expires: Dec 25 23:24:55 2026 GMT
  host: cloud.helios.id
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloud Helios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloud Helios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cloud Helios
provider_slug: cloud-helios
slug: cloud-helios-domain-security
source_filename: cloud-helios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.helios.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:24:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: helios.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud-helios/refs/heads/main/security/cloud-helios-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Management
- IT Security
- Cloud Services
- Cloud Infrastructure
- Business Continuity
---
