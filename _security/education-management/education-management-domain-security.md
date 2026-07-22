---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: education-management.com
  spf: true
hosts:
- cert_expires: Sep 17 23:22:13 2026 GMT
  host: www.education-management.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Education Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for education-management, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: education-management
provider_slug: education-management
slug: education-management-domain-security
source_filename: education-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.education-management.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:22:13 2026 GMT\n  hsts: false\ndomains:\n- domain: education-management.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/education-management/refs/heads/main/security/education-management-domain-security.yml
summary_line: TLSv1.3
tags: []
---
