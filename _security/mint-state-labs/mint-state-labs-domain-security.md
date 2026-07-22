---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mintstatelabs.com
  spf: true
hosts:
- cert_expires: Oct 12 12:46:03 2026 GMT
  host: mintstatelabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mint State Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mint State Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mint State Labs
provider_slug: mint-state-labs
slug: mint-state-labs-domain-security
source_filename: mint-state-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mintstatelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 12:46:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mintstatelabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mint-state-labs/refs/heads/main/security/mint-state-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Software Development
- IT Outsourcing
- Artificial Intelligence
- Machine Learning
- Consulting
- Cloud
- Staff Augmentation
---
