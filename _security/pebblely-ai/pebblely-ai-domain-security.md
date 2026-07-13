---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pebblely.com
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: pebblely.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pebblely Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pebblely AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pebblely AI
provider_slug: pebblely-ai
slug: pebblely-ai-domain-security
source_filename: pebblely-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pebblely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: pebblely.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pebblely-ai/refs/heads/main/security/pebblely-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- AI Photography
- Image Generation
- Product Photos
---
