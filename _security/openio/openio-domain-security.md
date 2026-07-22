---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openio.io
  spf: true
hosts:
- host: www.openio.io
  https: false
kind: domain-security
layout: security
method: probed
name: Openio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenIO, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenIO
provider_slug: openio
slug: openio-domain-security
source_filename: openio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openio.io\n  https: false\ndomains:\n- domain: openio.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openio/refs/heads/main/security/openio-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Infrastructure Saas
- Object Storage
- S3
- Cloud Storage
- Open Source
- OpenStack Swift
- Storage
---
