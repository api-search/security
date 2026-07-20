---
api_specs:
- filename: athenian-openapi-original.yml
  format: yaml
  label: Athenian API
  slug: athenian-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: athenian.com
  spf: true
hosts:
- cert_expires: Sep 24 10:43:36 2026 GMT
  host: athenian.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Athenian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Athenian, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Athenian
provider_slug: athenian
slug: athenian-domain-security
source_filename: athenian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: athenian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:43:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: athenian.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/security/athenian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Engineering Intelligence
- Software Development Analytics
- Developer Productivity
- DevOps
- Metrics
- Git
- JIRA
- CI/CD
- Analytics
---
