---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: data.gov.uk
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: coronavirus.data.gov.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coronavirus In The Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coronavirus in the UK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Coronavirus in the UK
provider_slug: coronavirus-in-the-uk
slug: coronavirus-in-the-uk-domain-security
source_filename: coronavirus-in-the-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coronavirus.data.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: data.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coronavirus-in-the-uk/refs/heads/main/security/coronavirus-in-the-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Health
- Public APIs
---
