---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: offenderlist.us
  spf: true
hosts:
- cert_expires: Aug 22 20:32:36 2026 GMT
  host: offenderlist.us
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Offenderlist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OffenderList, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OffenderList
provider_slug: offenderlist
slug: offenderlist-domain-security
source_filename: offenderlist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: offenderlist.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 20:32:36 2026 GMT\n  hsts: false\ndomains:\n- domain: offenderlist.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offenderlist/refs/heads/main/security/offenderlist-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sex Offenders
- Public Safety
- Criminal Records
---
