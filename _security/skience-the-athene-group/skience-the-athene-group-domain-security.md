---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: skience.com
  spf: true
hosts:
- cert_expires: Oct 12 03:04:42 2026 GMT
  host: www.skience.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skience The Athene Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skience (The Athene Group), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Skience (The Athene Group)
provider_slug: skience-the-athene-group
slug: skience-the-athene-group-domain-security
source_filename: skience-the-athene-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:04:42 2026 GMT\n  hsts: null\ndomains:\n- domain: skience.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skience-the-athene-group/refs/heads/main/security/skience-the-athene-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Wealth Management
- Financial Services
- WealthTech
- Salesforce
- Onboarding
- Account Opening
- Data Management
- SaaS
---
