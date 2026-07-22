---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: talentql.com
  spf: true
hosts:
- cert_expires: Aug 31 00:25:42 2026 GMT
  host: talentql.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Talentql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TalentQL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TalentQL
provider_slug: talentql
slug: talentql-domain-security
source_filename: talentql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talentql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 00:25:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: talentql.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talentql/refs/heads/main/security/talentql-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
