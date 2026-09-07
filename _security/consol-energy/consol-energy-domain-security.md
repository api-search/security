---
api_specs:
- filename: consol-energy-mines-content-api-openapi.yml
  format: yaml
  label: Core Natural Resources Mines Content API
  slug: mines-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consol-energy/refs/heads/main/openapi/consol-energy-mines-content-api-openapi.yml
- filename: consol-energy-leadership-content-api-openapi.yml
  format: yaml
  label: Core Natural Resources Leadership Content API
  slug: leadership-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consol-energy/refs/heads/main/openapi/consol-energy-leadership-content-api-openapi.yml
- filename: consol-energy-news-content-api-openapi.yml
  format: yaml
  label: Core Natural Resources News Content API
  slug: news-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consol-energy/refs/heads/main/openapi/consol-energy-news-content-api-openapi.yml
- filename: consol-energy-site-content-api-openapi.yml
  format: yaml
  label: Core Natural Resources Site Content API
  slug: site-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consol-energy/refs/heads/main/openapi/consol-energy-site-content-api-openapi.yml
- filename: consol-energy-discovery-api-openapi.yml
  format: yaml
  label: Core Natural Resources Discovery API
  slug: discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consol-energy/refs/heads/main/openapi/consol-energy-discovery-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: corenaturalresources.com
  spf: false
- caa:
  - 0 issue "entrust.net"
  - 0 iodef "mailto:CAIssues@sec.gov"
  - 0 issuewild ";"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sec.gov
  spf: true
hosts:
- cert_expires: Oct 12 05:02:30 2026 GMT
  host: corenaturalresources.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.sec.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Consol Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CONSOL Energy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CONSOL Energy
provider_slug: consol-energy
slug: consol-energy-domain-security
source_filename: consol-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corenaturalresources.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 05:02:30 2026 GMT\n  hsts: false\n- host: www.sec.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: corenaturalresources.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: sec.gov\n  dnssec: true\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 iodef \"mailto:CAIssues@sec.gov\"\n  - 0 issuewild \";\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consol-energy/refs/heads/main/security/consol-energy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Bituminous Coal
- Coal Mining
- Core Natural Resources
- Energy
- Investor Relations
- Mining
- Suppliers
- Sustainability
- Fortune 1000
---
