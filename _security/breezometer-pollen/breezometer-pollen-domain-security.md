---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: breezometer.com
  spf: true
hosts:
- cert_expires: Aug 29 18:13:18 2026 GMT
  host: docs.breezometer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Breezometer Pollen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BreezoMeter Pollen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BreezoMeter Pollen
provider_slug: breezometer-pollen
slug: breezometer-pollen-domain-security
source_filename: breezometer-pollen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.breezometer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 18:13:18 2026 GMT\n  hsts: false\ndomains:\n- domain: breezometer.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breezometer-pollen/refs/heads/main/security/breezometer-pollen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Environment
- Public APIs
---
