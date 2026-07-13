---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usagm.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: opentech.fund
  spf: true
hosts:
- cert_expires: Aug  2 18:44:00 2026 GMT
  host: www.usagm.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 10:05:16 2026 GMT
  host: www.opentech.fund
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: U S Agency For Global Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for U.S. Agency for Global Media, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: U.S. Agency for Global Media
provider_slug: u-s-agency-for-global-media
slug: u-s-agency-for-global-media-domain-security
source_filename: u-s-agency-for-global-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usagm.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 18:44:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.opentech.fund\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 10:05:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: usagm.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: opentech.fund\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/u-s-agency-for-global-media/refs/heads/main/security/u-s-agency-for-global-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Media
- Broadcasting
- International
- Press Freedom
- Internet Freedom
---
