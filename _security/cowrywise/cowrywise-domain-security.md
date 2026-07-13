---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cowrywise.com
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: cowrywise.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: developers.cowrywise.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: production.embed.cowrywise.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cowrywise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cowrywise, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cowrywise
provider_slug: cowrywise
slug: cowrywise-domain-security
source_filename: cowrywise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cowrywise.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\n- host: developers.cowrywise.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\n- host: production.embed.cowrywise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cowrywise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cowrywise/refs/heads/main/security/cowrywise-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Fintech
- Wealth Management
- Investments
- Savings
- Mutual Funds
- Nigeria
- Africa
- Financial Services
- REST API
---
