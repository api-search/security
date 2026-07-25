---
api_specs:
- filename: chief-financial-officers-council-agencies-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Agencies API
  slug: chief-financial-officers-council-agencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-agencies-api-openapi.yml
- filename: chief-financial-officers-council-awards-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Awards API
  slug: chief-financial-officers-council-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-awards-api-openapi.yml
- filename: chief-financial-officers-council-downloads-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Downloads API
  slug: chief-financial-officers-council-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-downloads-api-openapi.yml
- filename: chief-financial-officers-council-federal-accounts-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Federal Accounts API
  slug: chief-financial-officers-council-federal-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-federal-accounts-api-openapi.yml
- filename: chief-financial-officers-council-recipients-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Recipients API
  slug: chief-financial-officers-council-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-recipients-api-openapi.yml
- filename: chief-financial-officers-council-references-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council References API
  slug: chief-financial-officers-council-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-references-api-openapi.yml
- filename: chief-financial-officers-council-search-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Search API
  slug: chief-financial-officers-council-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-search-api-openapi.yml
- filename: chief-financial-officers-council-subawards-api-openapi.yml
  format: yaml
  label: Chief Financial Officers Council Subawards API
  slug: chief-financial-officers-council-subawards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/openapi/chief-financial-officers-council-subawards-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cfo.gov
  spf: true
- caa:
  - 0 issue "letsencrypt.org; accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/73686273"
  - 0 issuewild ";"
  - 0 issue "letsencrypt.org; accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/73686272"
  - 0 iodef "mailto:DL.OMB.MAXExtCerts@omb.eop.gov"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: paymentaccuracy.gov
  spf: true
hosts:
- host: www.cfo.gov
  https: false
- cert_expires: Aug 22 21:53:05 2026 GMT
  host: www.paymentaccuracy.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api.usaspending.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Chief Financial Officers Council Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chief Financial Officers Council, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Chief Financial Officers Council
provider_slug: chief-financial-officers-council
slug: chief-financial-officers-council-domain-security
source_filename: chief-financial-officers-council-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cfo.gov\n  https: false\n- host: www.paymentaccuracy.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 21:53:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usaspending.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cfo.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: paymentaccuracy.gov\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org; accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/73686273\"\n  - 0 issuewild \";\"\n  - 0 issue \"letsencrypt.org; accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/73686272\"\n  - 0 iodef \"mailto:DL.OMB.MAXExtCerts@omb.eop.gov\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chief-financial-officers-council/refs/heads/main/security/chief-financial-officers-council-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Financial Management
- Federal Government
- Finance
- Government
- OMB
- Treasury
---
