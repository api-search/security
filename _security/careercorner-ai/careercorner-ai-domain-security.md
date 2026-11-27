---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: careercorner.ai
  spf: true
hosts:
- cert_expires: Dec 25 15:20:02 2026 GMT
  host: careercorner.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CareerCorner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CareerCorner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CareerCorner
provider_slug: careercorner-ai
slug: careercorner-ai-domain-security
source_filename: careercorner-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: careercorner.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 15:20:02 2026 GMT\n  hsts: null\ndomains:\n- domain: careercorner.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/careercorner-ai/security/careercorner-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Job Search
- Coaching
- Careers
- Platform
- Company
---
