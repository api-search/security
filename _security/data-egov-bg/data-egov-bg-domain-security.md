---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: egov.bg
  spf: true
hosts:
- cert_expires: Aug 10 19:35:15 2026 GMT
  host: data.egov.bg
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Data Egov Bg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for data.egov.bg (Open Data Portal of Bulgaria), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: data.egov.bg (Open Data Portal of Bulgaria)
provider_slug: data-egov-bg
slug: data-egov-bg-domain-security
source_filename: data-egov-bg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.egov.bg\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 10 19:35:15 2026 GMT\n  hsts: null\ndomains:\n- domain: egov.bg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-egov-bg/refs/heads/main/security/data-egov-bg-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Open Data
- Custom Platform
- REST
- Government Data
- National Government
- Bulgaria
- Europe
---
