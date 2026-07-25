---
api_specs:
- filename: sas-businessrules-api-openapi.yml
  format: yaml
  label: SAS Institute BusinessRules API
  slug: sas-businessrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-businessrules-api-openapi.yml
- filename: sas-cas-api-openapi.yml
  format: yaml
  label: SAS Institute CAS API
  slug: sas-cas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-cas-api-openapi.yml
- filename: sas-decisions-api-openapi.yml
  format: yaml
  label: SAS Institute Decisions API
  slug: sas-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-decisions-api-openapi.yml
- filename: sas-files-api-openapi.yml
  format: yaml
  label: SAS Institute Files API
  slug: sas-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-files-api-openapi.yml
- filename: sas-folders-api-openapi.yml
  format: yaml
  label: SAS Institute Folders API
  slug: sas-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-folders-api-openapi.yml
- filename: sas-identities-api-openapi.yml
  format: yaml
  label: SAS Institute Identities API
  slug: sas-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-identities-api-openapi.yml
- filename: sas-jobs-api-openapi.yml
  format: yaml
  label: SAS Institute Jobs API
  slug: sas-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-jobs-api-openapi.yml
- filename: sas-logon-api-openapi.yml
  format: yaml
  label: SAS Institute Logon API
  slug: sas-logon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-logon-api-openapi.yml
- filename: sas-models-api-openapi.yml
  format: yaml
  label: SAS Institute Models API
  slug: sas-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-models-api-openapi.yml
- filename: sas-reports-api-openapi.yml
  format: yaml
  label: SAS Institute Reports API
  slug: sas-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-reports-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sas.com
  spf: true
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: www.sas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: developer.sas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAS Institute, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SAS Institute
provider_slug: sas
slug: sas-domain-security
source_filename: sas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sas.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.sas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sas.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/security/sas-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Data Management
- Artificial Intelligence
- Machine Learning
- Software
---
