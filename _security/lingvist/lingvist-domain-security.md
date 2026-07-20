---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:administrator@lingvist.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lingvist.com
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: lingvist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lingvist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lingvist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lingvist
provider_slug: lingvist
slug: lingvist-domain-security
source_filename: lingvist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lingvist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lingvist.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:administrator@lingvist.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lingvist/refs/heads/main/security/lingvist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Language Learning
- EdTech
- Artificial Intelligence
- Machine Learning
- Spaced Repetition
- Mobile
- Estonia
- Consumer
---
