---
description: ''
domains:
- caa:
  - n58jvl3e.up.railway.app.
  dmarc: false
  dnssec: true
  domain: manusai.ai
  spf: true
hosts:
- host: manusai.ai
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''manusai.ai'''
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Manusai Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Meta
provider_slug: manusai-ai
slug: manusai-ai-domain-security
source_filename: manusai-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manusai.ai\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''manusai.ai'''\n  hsts: null\ndomains:\n- domain: manusai.ai\n  dnssec: true\n  caa:\n  - n58jvl3e.up.railway.app.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/manusai-ai/security/manusai-ai-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- Technology
- Social Media
- Virtual Reality
- Artificial Intelligence
---
