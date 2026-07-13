---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: disease.sh
  spf: true
hosts:
- cert_expires: Oct  5 05:49:02 2026 GMT
  host: disease.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Disease Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Disease, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Open Disease
provider_slug: open-disease
slug: open-disease-domain-security
source_filename: open-disease-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: disease.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 05:49:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: disease.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-disease/refs/heads/main/security/open-disease-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Public APIs
---
