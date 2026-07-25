---
api_specs:
- filename: domaintools-flex-search-api-openapi.yml
  format: yaml
  label: DomainTools Flex search API
  slug: domaintools-flex-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-flex-search-api-openapi.yml
- filename: domaintools-information-api-openapi.yml
  format: yaml
  label: DomainTools Information API
  slug: domaintools-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-information-api-openapi.yml
- filename: domaintools-iris-detect-api-openapi.yml
  format: yaml
  label: DomainTools Iris Detect API
  slug: domaintools-iris-detect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-iris-detect-api-openapi.yml
- filename: domaintools-iris-enrich-api-openapi.yml
  format: yaml
  label: DomainTools Iris Enrich API
  slug: domaintools-iris-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-iris-enrich-api-openapi.yml
- filename: domaintools-iris-investigate-api-openapi.yml
  format: yaml
  label: DomainTools Iris Investigate API
  slug: domaintools-iris-investigate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-iris-investigate-api-openapi.yml
- filename: domaintools-lookups-api-openapi.yml
  format: yaml
  label: DomainTools Lookups API
  slug: domaintools-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-lookups-api-openapi.yml
- filename: domaintools-monitors-api-openapi.yml
  format: yaml
  label: DomainTools Monitors API
  slug: domaintools-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-monitors-api-openapi.yml
- filename: domaintools-ping-api-openapi.yml
  format: yaml
  label: DomainTools Ping API
  slug: domaintools-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-ping-api-openapi.yml
- filename: domaintools-rate-limit-api-openapi.yml
  format: yaml
  label: DomainTools Rate Limit API
  slug: domaintools-rate-limit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-rate-limit-api-openapi.yml
- filename: domaintools-rdata-lookups-api-openapi.yml
  format: yaml
  label: DomainTools rdata Lookups API
  slug: domaintools-rdata-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-rdata-lookups-api-openapi.yml
- filename: domaintools-rrset-lookups-api-openapi.yml
  format: yaml
  label: DomainTools rrset Lookups API
  slug: domaintools-rrset-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-rrset-lookups-api-openapi.yml
- filename: domaintools-siebatchd-api-openapi.yml
  format: yaml
  label: DomainTools Siebatchd API
  slug: domaintools-siebatchd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-siebatchd-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: dnsdb.info
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: fsi.io
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.dnsdb.info
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: dnsdbfront.labs.fsi.io
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api.domaintools.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Domaintools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DomainTools, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: DomainTools
provider_slug: domaintools
slug: domaintools-domain-security
source_filename: domaintools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.dnsdb.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dnsdbfront.labs.fsi.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: null\n- host: api.domaintools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dnsdb.info\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n- domain: fsi.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/security/domaintools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Threat Intelligence
- Domain Intelligence
- DNS
- WHOIS
- Passive DNS
- Cybersecurity
- Domain Monitoring
- Risk Scoring
- Security
---
