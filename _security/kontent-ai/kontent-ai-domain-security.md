---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@kontent.ai"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kontent.ai
  spf: true
hosts:
- cert_expires: Sep  4 14:38:54 2026 GMT
  host: kontent.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 14:38:54 2026 GMT
  host: deliver.kontent.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 14:38:54 2026 GMT
  host: preview-deliver.kontent.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kontent Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kontent AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kontent AI
provider_slug: kontent-ai
slug: kontent-ai-domain-security
source_filename: kontent-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kontent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 14:38:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: deliver.kontent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 14:38:54 2026 GMT\n  hsts: null\n- host: preview-deliver.kontent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 14:38:54 2026 GMT\n  hsts: null\ndomains:\n- domain: kontent.ai\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@kontent.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kontent-ai/refs/heads/main/security/kontent-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CMS
- Content
- GraphQL
- Headless CMS
---
