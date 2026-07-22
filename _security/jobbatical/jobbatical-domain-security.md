---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jobbatical.com
  spf: true
hosts:
- cert_expires: Aug 25 18:25:03 2026 GMT
  host: jobbatical.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jobbatical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jobbatical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jobbatical
provider_slug: jobbatical
slug: jobbatical-domain-security
source_filename: jobbatical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobbatical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 18:25:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: jobbatical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jobbatical/refs/heads/main/security/jobbatical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Immigration
- Global Mobility
- Relocation
- Visas
- Work Permits
- HR
- Compliance
- SaaS
---
