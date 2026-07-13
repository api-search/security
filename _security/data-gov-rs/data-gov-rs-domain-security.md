---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: data.gov.rs
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: data.gov.rs
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Data Gov Rs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for data.gov.rs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: data.gov.rs
provider_slug: data-gov-rs
slug: data-gov-rs-domain-security
source_filename: data-gov-rs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.gov.rs\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: data.gov.rs\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-gov-rs/refs/heads/main/security/data-gov-rs-domain-security.yml
summary_line: TLSv1.2
tags:
- Open Data
- uData
- Data Catalog
- DCAT
- Government Data
- National Government
- Serbia
- Europe
---
