---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: atomicmachines.com
  spf: true
hosts:
- cert_expires: Dec  9 04:32:54 2026 GMT
  host: www.atomicmachines.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atomic Machines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atomic Machines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Atomic Machines
provider_slug: atomic-machines
slug: atomic-machines-domain-security
source_filename: atomic-machines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atomicmachines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 04:32:54 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: atomicmachines.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomic-machines/refs/heads/main/security/atomic-machines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Manufacturing
- Robotics
- Automation
- Silicon
- MEMS
---
