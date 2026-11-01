---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: readeck.org
  spf: true
hosts:
- cert_expires: Jan 24 08:16:10 2027 GMT
  host: readeck.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Readeck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Readeck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Readeck
provider_slug: readeck
slug: readeck-domain-security
source_filename: readeck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: readeck.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 08:16:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: readeck.org\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/readeck/security/readeck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Reading
- Content Curation
- Bookmarking
- Productivity
---
