---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: osf.io
  spf: true
hosts:
- cert_expires: Aug 24 00:48:30 2026 GMT
  host: share.osf.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Share Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SHARE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SHARE
provider_slug: share
slug: share-domain-security
source_filename: share-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: share.osf.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 00:48:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: osf.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/share/refs/heads/main/security/share-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Science And Math
- Public APIs
---
