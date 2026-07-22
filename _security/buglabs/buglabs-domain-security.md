---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: buglabs.net
  spf: true
hosts:
- cert_expires: Oct 11 20:19:36 2026 GMT
  host: buglabs.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buglabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bug Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bug Labs
provider_slug: buglabs
slug: buglabs-domain-security
source_filename: buglabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buglabs.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 20:19:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: buglabs.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buglabs/refs/heads/main/security/buglabs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Enterprise Software
- Internet of Things
- Workflow Automation
- API Orchestration
- Networking
- Artificial Intelligence
- New York
---
