---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: precisionneuro.io
  spf: true
hosts:
- cert_expires: Sep 23 18:23:43 2026 GMT
  host: www.precisionneuro.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Precision Neuroscience Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Precision Neuroscience, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Precision Neuroscience
provider_slug: precision-neuroscience
slug: precision-neuroscience-domain-security
source_filename: precision-neuroscience-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.precisionneuro.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 18:23:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: precisionneuro.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/precision-neuroscience/refs/heads/main/security/precision-neuroscience-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- brain-computer-interface
- neurotechnology
- medical-devices
- neuroscience
- implantable-devices
- neural-interfaces
- health-technology
- clinical-research
- deep-tech
---
