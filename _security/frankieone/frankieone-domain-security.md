---
api_specs:
- filename: frankieone-audit-api-openapi.yml
  format: yaml
  label: FrankieOne Audit API
  slug: frankieone-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-audit-api-openapi.yml
- filename: frankieone-hostedurl-api-openapi.yml
  format: yaml
  label: FrankieOne HostedURL API
  slug: frankieone-hostedurl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-hostedurl-api-openapi.yml
- filename: frankieone-idv-api-openapi.yml
  format: yaml
  label: FrankieOne IDV API
  slug: frankieone-idv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-idv-api-openapi.yml
- filename: frankieone-individual-documents-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Documents API
  slug: frankieone-individual-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-documents-api-openapi.yml
- filename: frankieone-individual-entities-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Entities API
  slug: frankieone-individual-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-entities-api-openapi.yml
- filename: frankieone-individual-entity-elements-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Entity Elements API
  slug: frankieone-individual-entity-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-entity-elements-api-openapi.yml
- filename: frankieone-individual-profiles-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Profiles API
  slug: frankieone-individual-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-profiles-api-openapi.yml
- filename: frankieone-individual-results-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Results API
  slug: frankieone-individual-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-results-api-openapi.yml
- filename: frankieone-individual-risks-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Risks API
  slug: frankieone-individual-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-risks-api-openapi.yml
- filename: frankieone-individual-workflows-api-openapi.yml
  format: yaml
  label: FrankieOne Individual Workflows API
  slug: frankieone-individual-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-individual-workflows-api-openapi.yml
- filename: frankieone-matchlists-api-openapi.yml
  format: yaml
  label: FrankieOne Matchlists API
  slug: frankieone-matchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-matchlists-api-openapi.yml
- filename: frankieone-monitoring-api-openapi.yml
  format: yaml
  label: FrankieOne Monitoring API
  slug: frankieone-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-monitoring-api-openapi.yml
- filename: frankieone-search-api-openapi.yml
  format: yaml
  label: FrankieOne Search API
  slug: frankieone-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/openapi/frankieone-search-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "www.digicert.com"
  - 0 issue "docusign.fr"
  - 0 issue "godaddy.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: frankieone.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: frankie.one
  spf: false
hosts:
- cert_expires: Aug 24 10:55:16 2026 GMT
  host: www.frankieone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 13:40:20 2026 GMT
  host: docs.frankieone.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 06:07:12 2026 GMT
  host: api.frankie.one
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frankieone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FrankieOne, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: FrankieOne
provider_slug: frankieone
slug: frankieone-domain-security
source_filename: frankieone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.frankieone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:55:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.frankieone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:40:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.frankie.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:07:12 2026 GMT\n  hsts: null\ndomains:\n- domain: frankieone.com\n  dnssec: true\n  caa:\n  - 0 issue \"www.digicert.com\"\n  - 0 issue \"docusign.fr\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: frankie.one\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frankieone/refs/heads/main/security/frankieone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Identity Verification
- KYC
- KYB
- AML
- Fraud
- Compliance
---
