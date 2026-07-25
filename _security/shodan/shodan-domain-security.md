---
api_specs:
- filename: shodan-account-api-openapi.yml
  format: yaml
  label: Shodan Account API
  slug: shodan-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-account-api-openapi.yml
- filename: shodan-bulk-data-api-openapi.yml
  format: yaml
  label: Shodan Bulk Data API
  slug: shodan-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-bulk-data-api-openapi.yml
- filename: shodan-cpe-api-openapi.yml
  format: yaml
  label: Shodan CPE API
  slug: shodan-cpe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-cpe-api-openapi.yml
- filename: shodan-cve-api-openapi.yml
  format: yaml
  label: Shodan CVE API
  slug: shodan-cve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-cve-api-openapi.yml
- filename: shodan-directory-api-openapi.yml
  format: yaml
  label: Shodan Directory API
  slug: shodan-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-directory-api-openapi.yml
- filename: shodan-dns-api-openapi.yml
  format: yaml
  label: Shodan DNS API
  slug: shodan-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-dns-api-openapi.yml
- filename: shodan-internetdb-api-openapi.yml
  format: yaml
  label: Shodan InternetDB API
  slug: shodan-internetdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-internetdb-api-openapi.yml
- filename: shodan-network-alerts-api-openapi.yml
  format: yaml
  label: Shodan Network Alerts API
  slug: shodan-network-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-network-alerts-api-openapi.yml
- filename: shodan-notifiers-api-openapi.yml
  format: yaml
  label: Shodan Notifiers API
  slug: shodan-notifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-notifiers-api-openapi.yml
- filename: shodan-on-demand-scanning-api-openapi.yml
  format: yaml
  label: Shodan On-Demand Scanning API
  slug: shodan-on-demand-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-on-demand-scanning-api-openapi.yml
- filename: shodan-organization-api-openapi.yml
  format: yaml
  label: Shodan Organization API
  slug: shodan-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-organization-api-openapi.yml
- filename: shodan-search-methods-api-openapi.yml
  format: yaml
  label: Shodan Search Methods API
  slug: shodan-search-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-search-methods-api-openapi.yml
- filename: shodan-streaming-api-openapi.yml
  format: yaml
  label: Shodan Streaming API
  slug: shodan-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-streaming-api-openapi.yml
- filename: shodan-trends-api-openapi.yml
  format: yaml
  label: Shodan Trends API
  slug: shodan-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-trends-api-openapi.yml
- filename: shodan-utility-api-openapi.yml
  format: yaml
  label: Shodan Utility API
  slug: shodan-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shodan/refs/heads/main/openapi/shodan-utility-api-openapi.yml
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
