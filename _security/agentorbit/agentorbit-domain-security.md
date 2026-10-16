---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agentorbit.tech
  spf: false
hosts:
- host: agentorbit.tech
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''agentorbit.'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentorbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentOrbit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AgentOrbit
provider_slug: agentorbit
slug: agentorbit-domain-security
source_filename: agentorbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentorbit.tech\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''agentorbit.'\n  hsts: null\ndomains:\n- domain: agentorbit.tech\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentorbit/refs/heads/main/security/agentorbit-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- API
- SaaS
- Automation
- Integration
- Marketing
---
