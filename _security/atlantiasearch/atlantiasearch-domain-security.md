---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: atlantia.ai
  spf: false
hosts:
- cert_expires: Nov 25 17:48:37 2026 GMT
  host: www.atlantia.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atlantiasearch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atlantiasearch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Atlantiasearch
provider_slug: atlantiasearch
slug: atlantiasearch-domain-security
source_filename: atlantiasearch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atlantia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 17:48:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: atlantia.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlantiasearch/refs/heads/main/security/atlantiasearch-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Market Research
- Consumer Insights
- Data Analytics
- Software-as-a-Service
- Platform
---
