---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: seedlegals.com
  spf: true
hosts:
- cert_expires: Sep 14 11:21:28 2026 GMT
  host: seedlegals.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seedlegals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SeedLegals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SeedLegals
provider_slug: seedlegals
slug: seedlegals-domain-security
source_filename: seedlegals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seedlegals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 11:21:28 2026 GMT\n  hsts: false\ndomains:\n- domain: seedlegals.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seedlegals/refs/heads/main/security/seedlegals-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Business Applications
- Legal Tech
- Startups
- Fundraising
- Cap Table
- Equity
- Compliance
- MCP
- OpenID Connect
---
