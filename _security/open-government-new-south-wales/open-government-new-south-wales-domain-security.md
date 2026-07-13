---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nsw.gov.au
  spf: true
hosts:
- cert_expires: Oct  6 23:53:54 2026 GMT
  host: api.nsw.gov.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government New South Wales Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, New South Wales, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Open Government, New South Wales
provider_slug: open-government-new-south-wales
slug: open-government-new-south-wales-domain-security
source_filename: open-government-new-south-wales-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.nsw.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:53:54 2026 GMT\n  hsts: false\ndomains:\n- domain: nsw.gov.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-new-south-wales/refs/heads/main/security/open-government-new-south-wales-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Government
- Public APIs
---
