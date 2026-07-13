---
api_specs:
- filename: shodan-rest-openapi.yml
  format: yaml
  label: Shodan REST API
  slug: shodan-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-rest-openapi.yml
- filename: shodan-stream-openapi.yml
  format: yaml
  label: Shodan Streaming API
  slug: shodan-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-stream-openapi.yml
- filename: shodan-trends-openapi.yml
  format: yaml
  label: Shodan Trends API
  slug: shodan-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-trends-openapi.yml
- filename: shodan-internetdb-openapi.yml
  format: yaml
  label: InternetDB API
  slug: internetdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-internetdb-openapi.yml
- filename: shodan-cvedb-openapi.yml
  format: yaml
  label: CVEDB API
  slug: cvedb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-cvedb-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: shodan.io
  spf: true
hosts:
- cert_expires: Sep 18 10:18:31 2026 GMT
  host: www.shodan.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 10:18:31 2026 GMT
  host: developer.shodan.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 10:18:31 2026 GMT
  host: api.shodan.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shodan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shodan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Shodan
provider_slug: shodan
slug: shodan-domain-security
source_filename: shodan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shodan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:18:31 2026 GMT\n  hsts: false\n- host: developer.shodan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:18:31 2026 GMT\n  hsts: false\n- host: api.shodan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:18:31 2026 GMT\n  hsts: null\ndomains:\n- domain: shodan.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/security/shodan-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Security
- Search
- Internet
- Devices
- IoT
- Vulnerabilities
- CVE
- Attack Surface
- Threat Intelligence
- Reconnaissance
- Network
- DNS
- Scanning
- Public APIs
---
