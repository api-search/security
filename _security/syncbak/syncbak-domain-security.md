---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zeammedia.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zeam.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net ~all
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: syncbak.com
  note: DMARC rua aggregate-report mailbox is a named individual; not recorded here per the enrichment PII guardrail.
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:amazonses.com include:servers.mcsv.net ~all
hosts:
- cert_expires: Oct 22 22:36:08 2026 GMT
  host: zeammedia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: zeam.com
  hsts: false
  https: true
  note: Zeam consumer streaming app host (ASP.NET). No Strict-Transport-Security header returned.
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.syncbak.com
  hsts: false
  https: true
  note: Legacy Syncbak host on an AWS ELB; HTTP 301 to https://zeammedia.com/ for every path probed.
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: syncbak.com
  hsts: false
  https: false
  note: 'Apex TLS fails hostname verification: the certificate presents only CN=*.syncbak.com / SAN DNS:*.syncbak.com, which does not match the bare apex. Plain HTTP 302s to https://syncbak.com and therefore dead-ends for a strict client.'
kind: domain-security
layout: security
method: probed
name: Syncbak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syncbak, probed live across 4 host(s) and 3 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Syncbak
provider_slug: syncbak
slug: syncbak-domain-security
source_filename: syncbak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts; zeam.com / syncbak.com / www.syncbak.com\n  probed by hand (2026-08-29)\nhosts:\n- host: zeammedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 22:36:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: zeam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\n  note: Zeam consumer streaming app host (ASP.NET). No Strict-Transport-Security header returned.\n- host: www.syncbak.com\n  https: true\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\n  note: Legacy Syncbak host on an AWS ELB; HTTP 301 to https://zeammedia.com/ for every path probed.\n- host: syncbak.com\n  https: false\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\n  note: 'Apex TLS fails hostname verification: the certificate presents only CN=*.syncbak.com / SAN DNS:*.syncbak.com,\n    which does not match the bare\
  \ apex. Plain HTTP 302s to https://syncbak.com and therefore dead-ends\n    for a strict client.'\ndomains:\n- domain: zeammedia.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: zeam.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net ~all\n  dmarc: true\n  dmarc_policy: none\n- domain: syncbak.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:amazonses.com include:servers.mcsv.net ~all\n  dmarc: true\n  dmarc_policy: none\n  note: DMARC rua aggregate-report mailbox is a named individual; not recorded here per the enrichment\n    PII guardrail.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syncbak/refs/heads/main/security/syncbak-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Broadcasting
- Streaming
- Video
- Media
- OTT
- Television
- Advertising
- Local News
---
