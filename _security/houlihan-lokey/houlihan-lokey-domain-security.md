---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hl.com
  spf: true
hosts:
- cert_expires: Aug 20 17:50:45 2026 GMT
  host: www.hl.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.hl.com
  https: false
- host: api.hl.com
  https: false
kind: domain-security
layout: security
method: probed
name: Houlihan Lokey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Houlihan Lokey, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Houlihan Lokey
provider_slug: houlihan-lokey
slug: houlihan-lokey-domain-security
source_filename: houlihan-lokey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 17:50:45 2026 GMT\n  hsts: false\n- host: developer.hl.com\n  https: false\n- host: api.hl.com\n  https: false\ndomains:\n- domain: hl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/houlihan-lokey/refs/heads/main/security/houlihan-lokey-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Investment Banking
- Financial Advisory
- M&A
---
