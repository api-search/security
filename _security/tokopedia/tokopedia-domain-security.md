---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tokopedia.com
  spf: false
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: developer.tokopedia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tokopedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tokopedia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Tokopedia
provider_slug: tokopedia
slug: tokopedia-domain-security
source_filename: tokopedia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.tokopedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tokopedia.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tokopedia/refs/heads/main/security/tokopedia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Shopping
- Public APIs
---
