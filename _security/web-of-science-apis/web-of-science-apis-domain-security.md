---
api_specs:
- filename: web-of-science-starter-openapi.yml
  format: yaml
  label: Web of Science Starter API
  slug: web-of-science-starter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/web-of-science-apis/refs/heads/main/openapi/web-of-science-starter-openapi.yml
- filename: web-of-science-expanded-openapi.yml
  format: yaml
  label: Web of Science API Expanded
  slug: web-of-science-expanded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/web-of-science-apis/refs/heads/main/openapi/web-of-science-expanded-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clarivate.com
  spf: true
hosts:
- cert_expires: Sep 22 11:01:13 2026 GMT
  host: clarivate.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: developer.clarivate.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 18 21:10:49 2026 GMT
  host: api.clarivate.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Web Of Science Apis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Web of Science APIs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Web of Science APIs
provider_slug: web-of-science-apis
slug: web-of-science-apis-domain-security
source_filename: web-of-science-apis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clarivate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:01:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: developer.clarivate.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: false\n- host: api.clarivate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:10:49 2026 GMT\n  hsts: false\ndomains:\n- domain: clarivate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/web-of-science-apis/refs/heads/main/security/web-of-science-apis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Research
- Academic
- Bibliometrics
- Citations
- Science
- Scholarly
---
