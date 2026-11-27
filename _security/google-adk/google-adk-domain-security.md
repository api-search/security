---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adk.dev
  spf: true
hosts:
- cert_expires: Dec 28 20:24:51 2026 GMT
  host: adk.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Google Agent Development Kit (ADK) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Agent Development Kit (ADK), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Agent Development Kit (ADK)
provider_slug: google-adk
slug: google-adk-domain-security
source_filename: google-adk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adk.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 20:24:51 2026 GMT\n  hsts: false\ndomains:\n- domain: adk.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-adk/security/google-adk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Agents
- AI Automation
- Agent Frameworks
- Open Source
- SDK
- Multi-Agent Systems
- Gemini
---
