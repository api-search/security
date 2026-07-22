---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@klarity.ai"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: klarity.ai
  spf: true
hosts:
- cert_expires: Aug 19 12:49:04 2026 GMT
  host: www.klarity.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klarity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klarity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Klarity
provider_slug: klarity
slug: klarity-domain-security
source_filename: klarity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.klarity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 12:49:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: klarity.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@klarity.ai\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klarity/refs/heads/main/security/klarity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Business Process Management
- Process Intelligence
- Enterprise Software
- Document Automation
- Finance
- Governance Risk and Compliance
- Agents
---
