---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: taylorandfrancis.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tandfonline.com
  spf: true
hosts:
- cert_expires: Sep 17 10:03:33 2026 GMT
  host: taylorandfrancis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 05:31:48 2026 GMT
  host: www.tandfonline.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 17:33:03 2026 GMT
  host: www.taylorfrancis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taylor Francis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taylor & Francis, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Taylor & Francis
provider_slug: taylor-francis
slug: taylor-francis-domain-security
source_filename: taylor-francis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taylorandfrancis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 10:03:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.tandfonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 05:31:48 2026 GMT\n  hsts: null\n- host: www.taylorfrancis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 17:33:03 2026 GMT\n  hsts: null\ndomains:\n- domain: taylorandfrancis.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tandfonline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taylor-francis/refs/heads/main/security/taylor-francis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Academic
- Books
- Journals
- Metadata
- Publishing
- Research
- Text Mining
---
