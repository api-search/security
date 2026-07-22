---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: heptio.com
  spf: true
hosts:
- host: www.heptio.com
  https: false
kind: domain-security
layout: security
method: probed
name: Heptio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heptio, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Heptio
provider_slug: heptio
slug: heptio-domain-security
source_filename: heptio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heptio.com\n  https: false\ndomains:\n- domain: heptio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heptio/refs/heads/main/security/heptio-domain-security.yml
summary_line: DMARC
tags:
- Company
- Open Source
- Kubernetes
- Cloud Native
- Containers
- DevOps
- Infrastructure
- Defunct
- Acquired
---
