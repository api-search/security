---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yesno.wtf
  spf: true
hosts:
- cert_expires: Aug 15 03:58:45 2026 GMT
  host: yesno.wtf
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Yes No Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yes No, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Yes No
provider_slug: yes-no
slug: yes-no-domain-security
source_filename: yes-no-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yesno.wtf\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 15 03:58:45 2026 GMT\n  hsts: false\ndomains:\n- domain: yesno.wtf\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yes-no/refs/heads/main/security/yes-no-domain-security.yml
summary_line: TLSv1.2
tags:
- Test Data
- Public APIs
---
