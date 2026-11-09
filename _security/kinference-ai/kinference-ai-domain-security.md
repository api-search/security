---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kinference.ai
  spf: true
hosts:
- cert_expires: Dec  9 18:45:38 2026 GMT
  host: kinference.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kinference Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kinference, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kinference
provider_slug: kinference-ai
slug: kinference-ai-domain-security
source_filename: kinference-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kinference.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 18:45:38 2026 GMT\n  hsts: false\ndomains:\n- domain: kinference.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kinference-ai/security/kinference-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Inference
- Kubernetes
- vLLM
- LLM Gateway
- Rate Limiting
- Load Balancing
- Open Source
- Platform Engineering
---
