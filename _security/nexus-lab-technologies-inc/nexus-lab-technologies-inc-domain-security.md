---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nexuslab.fr
  spf: true
hosts:
- cert_expires: Sep 24 23:29:25 2026 GMT
  host: nexuslab.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexus Lab Technologies Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexus Lab Technologies, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nexus Lab Technologies, Inc.
provider_slug: nexus-lab-technologies-inc
slug: nexus-lab-technologies-inc-domain-security
source_filename: nexus-lab-technologies-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexuslab.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:29:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nexuslab.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexus-lab-technologies-inc/refs/heads/main/security/nexus-lab-technologies-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Aviation
- Sustainability
- Climate
- Machine Learning
- Contrails
- Flight Optimization
- Aerospace
---
