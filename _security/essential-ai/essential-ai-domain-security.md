---
description: ''
domains:
- caa:
  - 0 issue "\"letsencrypt.org\""
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: false
  dnssec: false
  domain: essential.ai
  spf: false
hosts:
- cert_expires: Sep 30 19:33:53 2026 GMT
  host: www.essential.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Essential Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Essential AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Essential AI
provider_slug: essential-ai
slug: essential-ai-domain-security
source_filename: essential-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.essential.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:33:53 2026 GMT\n  hsts: null\ndomains:\n- domain: essential.ai\n  dnssec: false\n  caa:\n  - 0 issue \"\\\"letsencrypt.org\\\"\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/essential-ai/refs/heads/main/security/essential-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- artificial-intelligence
- machine-learning
- large-language-models
- open-weight-models
- ai-research
- foundation-models
- training-datasets
- open-source
- generative-ai
- agentic-ai
---
