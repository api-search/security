---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atypicalai.com
  spf: true
hosts:
- cert_expires: Oct  6 08:54:47 2026 GMT
  host: www.atypicalai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atypical Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atypical AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Atypical AI
provider_slug: atypical-ai
slug: atypical-ai-domain-security
source_filename: atypical-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atypicalai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:54:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atypicalai.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atypical-ai/refs/heads/main/security/atypical-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Education
- EdTech
- Learning Science
- Generative AI
- Tutoring
- Exam Preparation
---
