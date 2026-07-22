---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 iodef "mailto:security@cognichip.ai"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cognichip.ai
  spf: true
hosts:
- cert_expires: Sep  6 13:58:55 2026 GMT
  host: cognichip.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cognichip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognichip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cognichip
provider_slug: cognichip
slug: cognichip-domain-security
source_filename: cognichip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cognichip.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 13:58:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cognichip.ai\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 iodef \"mailto:security@cognichip.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognichip/refs/heads/main/security/cognichip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductors
- Artificial Intelligence
- Chip Design
- EDA
- Foundation Models
- Machine Learning
---
