---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alcatraz.ai
  spf: true
hosts:
- cert_expires: Oct 14 13:55:53 2026 GMT
  host: www.alcatraz.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 04:47:27 2026 GMT
  host: support.alcatraz.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: platform.alcatraz.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Alcatraz Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alcatraz AI, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alcatraz AI
provider_slug: alcatraz-ai
slug: alcatraz-ai-domain-security
source_filename: alcatraz-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alcatraz.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 13:55:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.alcatraz.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:47:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.alcatraz.ai\n  https: false\ndomains:\n- domain: alcatraz.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alcatraz-ai/refs/heads/main/security/alcatraz-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Access Control
- Biometrics
- Facial Authentication
- Physical Security
- Identity
- Internet of Things
- Artificial Intelligence
---
