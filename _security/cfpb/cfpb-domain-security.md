---
api_specs:
- filename: cfpb-aggregations-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Aggregations API
  slug: cfpb-aggregations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-aggregations-api-openapi.yml
- filename: cfpb-complaints-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Complaints API
  slug: cfpb-complaints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-complaints-api-openapi.yml
- filename: cfpb-csv-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) CSV API
  slug: cfpb-csv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-csv-api-openapi.yml
- filename: cfpb-edits-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Edits API
  slug: cfpb-edits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-edits-api-openapi.yml
- filename: cfpb-filers-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Filers API
  slug: cfpb-filers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-filers-api-openapi.yml
- filename: cfpb-filings-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Filings API
  slug: cfpb-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-filings-api-openapi.yml
- filename: cfpb-health-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Health API
  slug: cfpb-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-health-api-openapi.yml
- filename: cfpb-institutions-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Institutions API
  slug: cfpb-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-institutions-api-openapi.yml
- filename: cfpb-submissions-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Submissions API
  slug: cfpb-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-submissions-api-openapi.yml
- filename: cfpb-trends-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Trends API
  slug: cfpb-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-trends-api-openapi.yml
- filename: cfpb-typeahead-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Typeahead API
  slug: cfpb-typeahead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-typeahead-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: consumerfinance.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cfpb.gov
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.consumerfinance.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: ffiec.cfpb.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cfpb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Consumer Financial Protection Bureau (CFPB), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Consumer Financial Protection Bureau (CFPB)
provider_slug: cfpb
slug: cfpb-domain-security
source_filename: cfpb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.consumerfinance.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\n- host: ffiec.cfpb.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: consumerfinance.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cfpb.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/security/cfpb-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Consumer Finance
- Government
- Complaints
- Mortgage
- HMDA
- Financial Data
- Regulatory
- Open Data
---
