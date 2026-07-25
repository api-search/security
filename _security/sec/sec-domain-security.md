---
api_specs:
- filename: sec-company-concept-api-openapi.yml
  format: yaml
  label: SEC EDGAR Company Concept API
  slug: sec-company-concept-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-company-concept-api-openapi.yml
- filename: sec-company-facts-api-openapi.yml
  format: yaml
  label: SEC EDGAR Company Facts API
  slug: sec-company-facts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-company-facts-api-openapi.yml
- filename: sec-edgar-operational-status-api-api-openapi.yml
  format: yaml
  label: SEC EDGAR EDGAR Operational Status API API
  slug: sec-edgar-operational-status-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-edgar-operational-status-api-api-openapi.yml
- filename: sec-filer-management-api-api-openapi.yml
  format: yaml
  label: SEC EDGAR Filer Management API API
  slug: sec-filer-management-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-filer-management-api-api-openapi.yml
- filename: sec-frames-api-openapi.yml
  format: yaml
  label: SEC EDGAR Frames API
  slug: sec-frames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-frames-api-openapi.yml
- filename: sec-search-api-openapi.yml
  format: yaml
  label: SEC EDGAR Search API
  slug: sec-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-search-api-openapi.yml
- filename: sec-submission-api-api-openapi.yml
  format: yaml
  label: SEC EDGAR Submission API API
  slug: sec-submission-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-submission-api-api-openapi.yml
- filename: sec-submission-status-api-api-openapi.yml
  format: yaml
  label: SEC EDGAR Submission Status API API
  slug: sec-submission-status-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-submission-status-api-api-openapi.yml
- filename: sec-submissions-api-openapi.yml
  format: yaml
  label: SEC EDGAR Submissions API
  slug: sec-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/openapi/sec-submissions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:CAIssues@sec.gov"
  - 0 issuewild ";"
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sec.gov
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.sec.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: data.sec.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: efts.sec.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SEC EDGAR, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SEC EDGAR
provider_slug: sec
slug: sec-domain-security
source_filename: sec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sec.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: data.sec.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\n- host: efts.sec.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sec.gov\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:CAIssues@sec.gov\"\n  - 0 issuewild \";\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sec/refs/heads/main/security/sec-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial Data
- SEC
- EDGAR
- Public Company Filings
- XBRL
- Regulatory
- Government
- Financial Reporting
- Company Submissions
- Securities
---
