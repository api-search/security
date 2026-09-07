---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xylem.com
  spf: true
hosts:
- cert_expires: Oct 14 07:28:51 2026 GMT
  host: www.xylem.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- headers:
    referrer-policy: no-referrer
    x-content-type-options: nosniff
    x-xss-protection: '0'
  host: cloud.xylem.com
  hsts: max-age=31536000 ; includeSubDomains
  https: true
  note: Read manually from a live 401 on https://cloud.xylem.com/xcloud/v1/users/ on 2026-09-04. The API host enforces HSTS with includeSubDomains; the marketing site does not send HSTS at all.
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Xylem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xylem, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Xylem
provider_slug: xylem
slug: xylem-domain-security
source_filename: xylem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of apis.yml + product API hosts\n  (probe-domain-security.py, plus a manual header read of cloud.xylem.com)\nhosts:\n- host: www.xylem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:28:51 2026 GMT\n  hsts: null\n- host: cloud.xylem.com\n  https: true\n  hsts: max-age=31536000 ; includeSubDomains\n  headers:\n    x-content-type-options: nosniff\n    referrer-policy: no-referrer\n    x-xss-protection: '0'\n  note: >-\n    Read manually from a live 401 on https://cloud.xylem.com/xcloud/v1/users/ on\n    2026-09-04. The API host enforces HSTS with includeSubDomains; the marketing site\n    does not send HSTS at all.\ndomains:\n- domain: xylem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xylem/refs/heads/main/security/xylem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 1000
- Water
- Water Technology
- Utilities
- Smart Metering
- Industrial IoT
- Water Quality
- Wastewater
- Manufacturing
---
