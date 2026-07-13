---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vuldb.com
  spf: true
hosts:
- cert_expires: Aug 17 00:47:01 2026 GMT
  host: vuldb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vuldb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VulDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VulDB
provider_slug: vuldb
slug: vuldb-domain-security
source_filename: vuldb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vuldb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 00:47:01 2026 GMT\n  hsts: null\ndomains:\n- domain: vuldb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vuldb/refs/heads/main/security/vuldb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Security
- Public APIs
---
