---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: restfulapi.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uci.edu
  spf: true
hosts:
- cert_expires: Sep  3 23:14:49 2026 GMT
  host: restfulapi.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: www.ics.uci.edu
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 26 05:12:18 2026 GMT
  host: spec.openapis.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REST, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: REST
provider_slug: rest
slug: rest-domain-security
source_filename: rest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: restfulapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 23:14:49 2026 GMT\n  hsts: false\n- host: www.ics.uci.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\n- host: spec.openapis.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:12:18 2026 GMT\n  hsts: false\ndomains:\n- domain: restfulapi.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: uci.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rest/refs/heads/main/security/rest-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- API Design
- Architecture
- HTTP
- REST
- RESTful
- Web Services
---
