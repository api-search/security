---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 iodef "mailto:security-notifications@day.ai"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: day.ai
  spf: true
hosts:
- cert_expires: Dec  5 00:23:42 2026 GMT
  host: day.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dayai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Day.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Day.ai
provider_slug: dayai
slug: dayai-domain-security
source_filename: dayai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: day.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 00:23:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: day.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:security-notifications@day.ai\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dayai/security/dayai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Automation
- Enterprise
- Productivity
- Platform
---
