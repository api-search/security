---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nextroll.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adroll.com
  spf: true
hosts:
- cert_expires: Jan 12 21:08:01 2027 GMT
  host: www.nextroll.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: apidocs.nextroll.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: services.adroll.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nextroll Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NextRoll, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NextRoll
provider_slug: nextroll
slug: nextroll-domain-security
source_filename: nextroll-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nextroll.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 12 21:08:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidocs.nextroll.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: services.adroll.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nextroll.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: adroll.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextroll/refs/heads/main/security/nextroll-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Marketing
- Account Based Marketing
- Retargeting
- Audiences
- Campaign Management
- Analytics
- Reporting
- MarTech
- Agents
---
