---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: traceloop.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714"
  - 0 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2185112545"
  dmarc: false
  dnssec: false
  domain: opentelemetry.io
  spf: false
hosts:
- cert_expires: Oct  1 20:48:08 2026 GMT
  host: www.traceloop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 18:28:58 2026 GMT
  host: opentelemetry.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openllmetry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenLLMetry, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenLLMetry
provider_slug: openllmetry
slug: openllmetry-domain-security
source_filename: openllmetry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.traceloop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:48:08 2026 GMT\n  hsts: null\n- host: opentelemetry.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:28:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: traceloop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: opentelemetry.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714\"\n  - 0 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2185112545\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openllmetry/refs/heads/main/security/openllmetry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Observability
- Open Source
- OpenTelemetry
- Tracing
- GenAI
---
