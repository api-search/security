---
api_specs:
- filename: free-law-project-alerts-api-openapi.yml
  format: yaml
  label: Free Law Project Alerts API
  slug: free-law-project-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-alerts-api-openapi.yml
- filename: free-law-project-case-law-api-openapi.yml
  format: yaml
  label: Free Law Project Case Law API
  slug: free-law-project-case-law-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-case-law-api-openapi.yml
- filename: free-law-project-citations-api-openapi.yml
  format: yaml
  label: Free Law Project Citations API
  slug: free-law-project-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-citations-api-openapi.yml
- filename: free-law-project-financial-disclosures-api-openapi.yml
  format: yaml
  label: Free Law Project Financial Disclosures API
  slug: free-law-project-financial-disclosures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-financial-disclosures-api-openapi.yml
- filename: free-law-project-judges-api-openapi.yml
  format: yaml
  label: Free Law Project Judges API
  slug: free-law-project-judges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-judges-api-openapi.yml
- filename: free-law-project-oral-arguments-api-openapi.yml
  format: yaml
  label: Free Law Project Oral Arguments API
  slug: free-law-project-oral-arguments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-oral-arguments-api-openapi.yml
- filename: free-law-project-pacer-api-openapi.yml
  format: yaml
  label: Free Law Project PACER API
  slug: free-law-project-pacer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-pacer-api-openapi.yml
- filename: free-law-project-recap-api-openapi.yml
  format: yaml
  label: Free Law Project RECAP API
  slug: free-law-project-recap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-recap-api-openapi.yml
- filename: free-law-project-search-api-openapi.yml
  format: yaml
  label: Free Law Project Search API
  slug: free-law-project-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-search-api-openapi.yml
- filename: free-law-project-tags-api-openapi.yml
  format: yaml
  label: Free Law Project Tags API
  slug: free-law-project-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/openapi/free-law-project-tags-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:caa-violations@free.law"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: free.law
  spf: true
- caa:
  - 0 iodef "mailto:caa-violations@free.law"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: courtlistener.com
  spf: true
hosts:
- cert_expires: Aug 30 04:33:52 2026 GMT
  host: free.law
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: www.courtlistener.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Free Law Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Free Law Project, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Free Law Project
provider_slug: free-law-project
slug: free-law-project-domain-security
source_filename: free-law-project-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: free.law\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 04:33:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.courtlistener.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: free.law\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa-violations@free.law\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: courtlistener.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa-violations@free.law\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/free-law-project/refs/heads/main/security/free-law-project-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Courts
- Justice
- Legal
- Transparency
---
