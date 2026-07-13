---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aporia.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coralogix.com
  spf: true
hosts:
- cert_expires: Sep 21 06:24:57 2026 GMT
  host: www.aporia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 21:11:27 2026 GMT
  host: coralogix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aporia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aporia, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aporia
provider_slug: aporia
slug: aporia-domain-security
source_filename: aporia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aporia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:24:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: coralogix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 21:11:27 2026 GMT\n  hsts: false\ndomains:\n- domain: aporia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: coralogix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aporia/refs/heads/main/security/aporia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Guardrails
- ML Observability
- LLM Monitoring
- Coralogix
- Acquired
- Hallucination Detection
- Policy Enforcement
---
