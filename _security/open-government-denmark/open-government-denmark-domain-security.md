---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: opendata.dk
  spf: true
hosts:
- cert_expires: Sep 15 12:44:38 2026 GMT
  host: www.opendata.dk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Denmark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Denmark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Open Government, Denmark
provider_slug: open-government-denmark
slug: open-government-denmark-domain-security
source_filename: open-government-denmark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opendata.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 12:44:38 2026 GMT\n  hsts: null\ndomains:\n- domain: opendata.dk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-denmark/refs/heads/main/security/open-government-denmark-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Government
- Public APIs
---
