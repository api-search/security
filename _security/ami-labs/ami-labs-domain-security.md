---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: amilabs.xyz
  spf: true
hosts:
- cert_expires: Aug 18 13:16:33 2026 GMT
  host: amilabs.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ami Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMI Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AMI Labs
provider_slug: ami-labs
slug: ami-labs-domain-security
source_filename: ami-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amilabs.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 13:16:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amilabs.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ami-labs/refs/heads/main/security/ami-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Ai Enterprise Software
- Artificial Intelligence
- Machine Learning
- World Models
- AI Research
- Robotics
- Automation
---
