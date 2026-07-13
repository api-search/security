---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: data.gov.au
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.data.gov.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Australia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Open Government, Australia
provider_slug: open-government-australia
slug: open-government-australia-domain-security
source_filename: open-government-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.data.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: data.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-australia/refs/heads/main/security/open-government-australia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Government
- Public APIs
---
