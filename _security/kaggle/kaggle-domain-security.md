---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kaggle.com
  spf: true
hosts:
- cert_expires: Aug 18 12:35:06 2026 GMT
  host: www.kaggle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kaggle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaggle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kaggle
provider_slug: kaggle
slug: kaggle-domain-security
source_filename: kaggle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kaggle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 12:35:06 2026 GMT\n  hsts: null\ndomains:\n- domain: kaggle.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaggle/refs/heads/main/security/kaggle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- Public APIs
---
