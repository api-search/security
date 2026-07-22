---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: snapdocs.com
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: snapdocs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Snapdocs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snapdocs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Snapdocs
provider_slug: snapdocs
slug: snapdocs-domain-security
source_filename: snapdocs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snapdocs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: snapdocs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapdocs/refs/heads/main/security/snapdocs-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Proptech
- Mortgage
- Real Estate
- Fintech
- eClosing
- Title and Settlement
- Notary
---
