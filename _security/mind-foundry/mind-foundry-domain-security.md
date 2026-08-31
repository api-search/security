---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mindfoundry.ai
  spf: true
hosts:
- cert_expires: Sep 30 20:26:24 2026 GMT
  host: www.mindfoundry.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mind Foundry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mind Foundry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mind Foundry
provider_slug: mind-foundry
slug: mind-foundry-domain-security
source_filename: mind-foundry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mindfoundry.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 20:26:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mindfoundry.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mind-foundry/refs/heads/main/security/mind-foundry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- Defence
- National Security
- Sensor Fusion
- Responsible AI
- Optimization
- United Kingdom
---
