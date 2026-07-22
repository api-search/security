---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: uscp.gov
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.uscp.gov
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: United States Capitol Police Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United States Capitol Police, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: United States Capitol Police
provider_slug: united-states-capitol-police
slug: united-states-capitol-police-domain-security
source_filename: united-states-capitol-police-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uscp.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: uscp.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-capitol-police/refs/heads/main/security/united-states-capitol-police-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Law Enforcement
- Legislative Branch
- Security
- Public Safety
---
