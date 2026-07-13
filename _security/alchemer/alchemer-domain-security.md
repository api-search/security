---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alchemer.com
  spf: true
hosts:
- cert_expires: Sep 23 11:24:19 2026 GMT
  host: www.alchemer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 14:57:17 2026 GMT
  host: apihelp.alchemer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: api.alchemer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alchemer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alchemer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alchemer
provider_slug: alchemer
slug: alchemer-domain-security
source_filename: alchemer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alchemer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 11:24:19 2026 GMT\n  hsts: null\n- host: apihelp.alchemer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 14:57:17 2026 GMT\n  hsts: false\n- host: api.alchemer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: alchemer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alchemer/refs/heads/main/security/alchemer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Survey
- Experience Management
- Feedback
- Data Collection
- Enterprise
- Forms
---
