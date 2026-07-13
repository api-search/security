---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: data.gov.uk
  spf: true
hosts:
- cert_expires: Dec 28 22:06:14 2026 GMT
  host: data.gov.uk
  hsts: true
  hsts_max_age: 60
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, UK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Open Government, UK
provider_slug: open-government-uk
slug: open-government-uk-domain-security
source_filename: open-government-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 22:06:14 2026 GMT\n  hsts: true\n  hsts_max_age: 60\ndomains:\n- domain: data.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-uk/refs/heads/main/security/open-government-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Government
- Public APIs
---
