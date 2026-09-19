---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bakerhughes.com
  spf: true
hosts:
- cert_expires: Dec 14 05:55:38 2026 GMT
  host: www.bakerhughes.com
  hsts: true
  hsts_max_age: 63072000
  hsts_measured: '2026-07-11'
  hsts_note: The 2026-09-17 re-probe reached only an Imperva/Incapsula challenge interstitial (200, ~850 bytes, no Strict-Transport-Security header), which is the WAF answering, not the origin. The origin's HSTS header (max-age=63072000) was observed by the 2026-07-11 probe; carried forward rather than downgraded on a WAF shell.
  https: true
  tls_version: TLSv1.3
  waf: Imperva/Incapsula
- host: developer.bakerhughes.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: 'Backstage developer portal; strict-transport-security: max-age=31536000; includeSubDomains observed 2026-09-17 on a real (non-challenge) response.'
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Baker Hughes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baker Hughes, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Baker Hughes
provider_slug: baker-hughes
slug: baker-hughes-domain-security
source_filename: baker-hughes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bakerhughes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 05:55:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_measured: '2026-07-11'\n  hsts_note: The 2026-09-17 re-probe reached only an Imperva/Incapsula challenge interstitial (200, ~850 bytes,\n    no Strict-Transport-Security header), which is the WAF answering, not the origin. The origin's HSTS header (max-age=63072000)\n    was observed by the 2026-07-11 probe; carried forward rather than downgraded\n    on a WAF shell.\n  waf: Imperva/Incapsula\n- host: developer.bakerhughes.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: 'Backstage developer portal; strict-transport-security: max-age=31536000; includeSubDomains observed 2026-09-17\n    on a real (non-challenge) response.'\ndomains:\n- domain: bakerhughes.com\n\
  \  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baker-hughes/refs/heads/main/security/baker-hughes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy Technology
- Industrial IoT
- Oil and Gas
- Asset Performance Management
- Digital Energy
- Fortune 500
---
