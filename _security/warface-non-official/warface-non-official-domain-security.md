---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wfstats.cf
  spf: true
hosts:
- cert_expires: Sep  4 07:00:20 2026 GMT
  host: api.wfstats.cf
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Warface Non Official Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Warface (non-official), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Warface (non-official)
provider_slug: warface-non-official
slug: warface-non-official-domain-security
source_filename: warface-non-official-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.wfstats.cf\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 07:00:20 2026 GMT\n  hsts: false\ndomains:\n- domain: wfstats.cf\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warface-non-official/refs/heads/main/security/warface-non-official-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
