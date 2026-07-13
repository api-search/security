---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apigovernance.dev
  spf: true
hosts:
- cert_expires: Oct  6 21:18:30 2026 GMT
  host: apigovernance.dev
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apigovernance Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIGovernance.Dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: APIGovernance.Dev
provider_slug: apigovernance-dev
slug: apigovernance-dev-domain-security
source_filename: apigovernance-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apigovernance.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:18:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: apigovernance.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apigovernance-dev/refs/heads/main/security/apigovernance-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Design
- API Governance
- Best Practices
- Compliance
- Guidelines
- Standards
---
