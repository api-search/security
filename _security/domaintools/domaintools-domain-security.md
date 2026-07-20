---
api_specs:
- filename: domaintools-iris-openapi.yml
  format: yaml
  label: DomainTools Iris API
  slug: domaintools-iris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-iris-openapi.yml
- filename: domaintools-lookups-monitors-openapi.yml
  format: yaml
  label: DomainTools Lookups and Monitors API
  slug: domaintools-lookups-and-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-lookups-monitors-openapi.yml
- filename: domaintools-dnsdb-openapi.yml
  format: yaml
  label: Farsight DNSDB Passive DNS API
  slug: farsight-dnsdb-passive-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-dnsdb-openapi.yml
- filename: domaintools-sie-openapi.yml
  format: yaml
  label: Farsight SIE Batch API
  slug: farsight-sie-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-sie-openapi.yml
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
