---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: corma.io
  spf: true
hosts:
- cert_expires: Sep 17 22:18:17 2026 GMT
  host: www.corma.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Corma
provider_slug: corma
slug: corma-domain-security
source_filename: corma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.corma.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:18:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: corma.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corma/refs/heads/main/security/corma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Access Governance
- Cost Optimization
- Deprovisioning
- Identity Access Management
- License Management
- Provisioning
- SaaS Management
- SaaS Operations
- Shadow IT
- SMP
---
