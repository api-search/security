---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: whatthecommit.com
  spf: true
hosts:
- cert_expires: Aug 17 06:59:09 2026 GMT
  host: whatthecommit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: What The Commit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for What The Commit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: What The Commit
provider_slug: what-the-commit
slug: what-the-commit-domain-security
source_filename: what-the-commit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whatthecommit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 06:59:09 2026 GMT\n  hsts: null\ndomains:\n- domain: whatthecommit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/what-the-commit/refs/heads/main/security/what-the-commit-domain-security.yml
summary_line: TLSv1.3
tags:
- Test Data
- Public APIs
---
