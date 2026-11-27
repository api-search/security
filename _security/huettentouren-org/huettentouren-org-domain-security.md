---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: huettentouren.org
  spf: true
hosts:
- cert_expires: Jan 13 17:58:00 2027 GMT
  host: huettentouren.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: huettentouren-org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for huettentouren-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: huettentouren-org
provider_slug: huettentouren-org
slug: huettentouren-org-domain-security
source_filename: huettentouren-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: huettentouren.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 17:58:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: huettentouren.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/huettentouren-org/security/huettentouren-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
