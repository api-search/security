---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clarivate.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cortellis.com
  spf: false
hosts:
- cert_expires: Sep 22 11:01:13 2026 GMT
  host: clarivate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: developer.clarivate.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 25 04:42:34 2026 GMT
  host: www.cortellis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clarivate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clarivate, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Clarivate
provider_slug: clarivate
slug: clarivate-domain-security
source_filename: clarivate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clarivate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:01:13 2026 GMT\n  hsts: null\n- host: developer.clarivate.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: false\n- host: www.cortellis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 04:42:34 2026 GMT\n  hsts: false\ndomains:\n- domain: clarivate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cortellis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarivate/refs/heads/main/security/clarivate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Citations
- Data
- Drug Pipeline
- Insights
- Intellectual Property
- Life Sciences
- Patents
- Publications
- Research
---
