---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: domainsdb.info
  spf: false
hosts:
- cert_expires: Oct  9 16:17:01 2026 GMT
  host: domainsdb.info
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Domainsdb Info Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Domainsdb.info, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Domainsdb.info
provider_slug: domainsdb-info
slug: domainsdb-info-domain-security
source_filename: domainsdb-info-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domainsdb.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:17:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: domainsdb.info\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domainsdb-info/refs/heads/main/security/domainsdb-info-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Business
- Public APIs
---
