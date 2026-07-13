---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: data.gov.sg
  spf: true
hosts:
- cert_expires: Sep 13 07:45:57 2026 GMT
  host: data.gov.sg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Singapore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Singapore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Open Government, Singapore
provider_slug: open-government-singapore
slug: open-government-singapore-domain-security
source_filename: open-government-singapore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.gov.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 07:45:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: data.gov.sg\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-singapore/refs/heads/main/security/open-government-singapore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Public APIs
---
