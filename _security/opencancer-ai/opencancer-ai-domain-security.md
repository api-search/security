---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opencancer.ai
  spf: true
hosts:
- cert_expires: Dec 30 15:34:43 2026 GMT
  host: opencancer.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenCancer.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenCancer.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenCancer.ai
provider_slug: opencancer-ai
slug: opencancer-ai-domain-security
source_filename: opencancer-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opencancer.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 15:34:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: opencancer.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/opencancer-ai/security/opencancer-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Healthcare
- Cancer
- Patient Support
---
