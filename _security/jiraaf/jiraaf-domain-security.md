---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jiraaf.com
  spf: true
hosts:
- cert_expires: Sep  7 01:46:44 2026 GMT
  host: www.jiraaf.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jiraaf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jiraaf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Jiraaf
provider_slug: jiraaf
slug: jiraaf-domain-security
source_filename: jiraaf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jiraaf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 01:46:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: jiraaf.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jiraaf/refs/heads/main/security/jiraaf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Bonds
- Fixed Income
- Investing
- Wealth Management
- India
---
