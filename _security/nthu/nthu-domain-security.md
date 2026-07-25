---
api_specs:
- filename: nthu-announcements-api-openapi.yml
  format: yaml
  label: National Tsing Hua University Announcements API
  slug: nthu-announcements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/nthu-announcements-api-openapi.yml
- filename: nthu-buses-api-openapi.yml
  format: yaml
  label: National Tsing Hua University Buses API
  slug: nthu-buses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/nthu-buses-api-openapi.yml
- filename: nthu-courses-api-openapi.yml
  format: yaml
  label: National Tsing Hua University Courses API
  slug: nthu-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/nthu-courses-api-openapi.yml
- filename: nthu-departments-api-openapi.yml
  format: yaml
  label: National Tsing Hua University Departments API
  slug: nthu-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/nthu-departments-api-openapi.yml
- filename: nthu-dining-api-openapi.yml
  format: yaml
  label: National Tsing Hua University Dining API
  slug: nthu-dining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/nthu-dining-api-openapi.yml
- filename: nthu-energy-api-openapi.yml
  format: yaml
  label: National Tsing Hua University Energy API
  slug: nthu-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/nthu-energy-api-openapi.yml
- filename: nthu-libraries-api-openapi.yml
  format: yaml
  label: National Tsing Hua University Libraries API
  slug: nthu-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/nthu-libraries-api-openapi.yml
- filename: nthu-locations-api-openapi.yml
  format: yaml
  label: National Tsing Hua University Locations API
  slug: nthu-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/nthu-locations-api-openapi.yml
- filename: nthu-newsletters-api-openapi.yml
  format: yaml
  label: National Tsing Hua University Newsletters API
  slug: nthu-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/nthu-newsletters-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nthu.edu.tw
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: nthusa.tw
  spf: false
hosts:
- host: www.nthu.edu.tw
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Missing Subject Key Identifier (_ssl.c:1082)'
- cert_expires: Aug 25 02:04:51 2026 GMT
  host: api.nthusa.tw
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nthu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Tsing Hua University, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: National Tsing Hua University
provider_slug: nthu
slug: nthu-domain-security
source_filename: nthu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nthu.edu.tw\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Missing Subject\n    Key Identifier (_ssl.c:1082)'\n  hsts: null\n- host: api.nthusa.tw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 02:04:51 2026 GMT\n  hsts: null\ndomains:\n- domain: nthu.edu.tw\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nthusa.tw\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/security/nthu-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Taiwan
- Open Data
- Campus
---
