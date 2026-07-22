---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getenjoyhq.com
  spf: true
hosts:
- cert_expires: Aug 26 04:48:43 2026 GMT
  host: getenjoyhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Enjoyhq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EnjoyHQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EnjoyHQ
provider_slug: enjoyhq
slug: enjoyhq-domain-security
source_filename: enjoyhq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getenjoyhq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 26 04:48:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getenjoyhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enjoyhq/refs/heads/main/security/enjoyhq-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- User Research
- Customer Feedback
- Insights Management
- Research Repository
- User Experience
- Product Management
- SaaS
---
