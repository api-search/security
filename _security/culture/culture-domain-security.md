---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: culturepartners.com
  spf: true
hosts:
- cert_expires: Jan  6 06:01:10 2027 GMT
  host: culturepartners.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Culture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Culture, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Culture
provider_slug: culture
slug: culture-domain-security
source_filename: culture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: culturepartners.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 06:01:10 2027 GMT\n  hsts: false\ndomains:\n- domain: culturepartners.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culture/refs/heads/main/security/culture-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consulting
- OrganizationalCulture
- ChangeManagement
- Leadership
---
