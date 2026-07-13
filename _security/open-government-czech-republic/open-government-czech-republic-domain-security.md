---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: data.gov.cz
  spf: false
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: data.gov.cz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Czech Republic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Czech Republic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Government, Czech Republic
provider_slug: open-government-czech-republic
slug: open-government-czech-republic-domain-security
source_filename: open-government-czech-republic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.gov.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: data.gov.cz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-czech-republic/refs/heads/main/security/open-government-czech-republic-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Government
- Public APIs
---
