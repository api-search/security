---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: levocred.com
  spf: true
hosts:
- cert_expires: Sep 28 22:35:32 2026 GMT
  host: www.levocred.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: app.levocred.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 06:51:45 2026 GMT
  host: trust.levocred.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Levocred Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Levocred AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Levocred AI
provider_slug: levocred-ai
slug: levocred-ai-domain-security
source_filename: levocred-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.levocred.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 22:35:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.levocred.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: trust.levocred.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 06:51:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: levocred.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levocred-ai/refs/heads/main/security/levocred-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Financial Services
- Private Credit
- Lending
- Credit Risk
- Fintech
- Y Combinator
---
