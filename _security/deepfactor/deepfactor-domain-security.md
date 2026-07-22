---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deepfactor.io
  spf: true
hosts:
- host: www.deepfactor.io
  https: false
kind: domain-security
layout: security
method: probed
name: Deepfactor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for deepfactor, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: deepfactor
provider_slug: deepfactor
slug: deepfactor-domain-security
source_filename: deepfactor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deepfactor.io\n  https: false\ndomains:\n- domain: deepfactor.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepfactor/refs/heads/main/security/deepfactor-domain-security.yml
summary_line: DMARC
tags:
- Company
- Cybersecurity
- Application Security
- DevSecOps
- SBOM
- Software Composition Analysis
- Container Security
- Supply Chain Security
- Cloud Native
---
