---
api_specs:
- filename: university-of-padua-datastream-api-openapi.yml
  format: yaml
  label: University of Padua datastream API
  slug: university-of-padua-datastream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-datastream-api-openapi.yml
- filename: university-of-padua-directory-api-openapi.yml
  format: yaml
  label: University of Padua directory API
  slug: university-of-padua-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-directory-api-openapi.yml
- filename: university-of-padua-imageserver-api-openapi.yml
  format: yaml
  label: University of Padua imageserver API
  slug: university-of-padua-imageserver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-imageserver-api-openapi.yml
- filename: university-of-padua-lists-api-openapi.yml
  format: yaml
  label: University of Padua lists API
  slug: university-of-padua-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-lists-api-openapi.yml
- filename: university-of-padua-misc-api-openapi.yml
  format: yaml
  label: University of Padua misc API
  slug: university-of-padua-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-misc-api-openapi.yml
- filename: university-of-padua-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Padua oai-pmh API
  slug: university-of-padua-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-oai-pmh-api-openapi.yml
- filename: university-of-padua-object-advanced-api-openapi.yml
  format: yaml
  label: University of Padua object-advanced API
  slug: university-of-padua-object-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-object-advanced-api-openapi.yml
- filename: university-of-padua-object-basics-api-openapi.yml
  format: yaml
  label: University of Padua object-basics API
  slug: university-of-padua-object-basics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-object-basics-api-openapi.yml
- filename: university-of-padua-relationships-api-openapi.yml
  format: yaml
  label: University of Padua relationships API
  slug: university-of-padua-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-relationships-api-openapi.yml
- filename: university-of-padua-search-api-openapi.yml
  format: yaml
  label: University of Padua search API
  slug: university-of-padua-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-search-api-openapi.yml
- filename: university-of-padua-session-api-openapi.yml
  format: yaml
  label: University of Padua session API
  slug: university-of-padua-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-session-api-openapi.yml
- filename: university-of-padua-stats-api-openapi.yml
  format: yaml
  label: University of Padua stats API
  slug: university-of-padua-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-stats-api-openapi.yml
- filename: university-of-padua-templates-api-openapi.yml
  format: yaml
  label: University of Padua templates API
  slug: university-of-padua-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-templates-api-openapi.yml
- filename: university-of-padua-vocabularies-api-openapi.yml
  format: yaml
  label: University of Padua vocabularies API
  slug: university-of-padua-vocabularies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/openapi/university-of-padua-vocabularies-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "harica.gr"
  - 0 iodef "mailto:admin.certificati@unipd.it"
  - 0 issuewild "harica.gr"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unipd.it
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: www.unipd.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 08:55:15 2026 GMT
  host: phaidra.cab.unipd.it
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
- host: paduaresearch.cab.unipd.it
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''paduaresear'
kind: domain-security
layout: security
method: probed
name: University Of Padua Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Padua, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Padua
provider_slug: university-of-padua
slug: university-of-padua-domain-security
source_filename: university-of-padua-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unipd.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: phaidra.cab.unipd.it\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 08:55:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: paduaresearch.cab.unipd.it\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''paduaresear'\n  hsts: null\ndomains:\n- domain: unipd.it\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"harica.gr\"\n  - 0 iodef \"mailto:admin.certificati@unipd.it\"\n  - 0 issuewild \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-padua/refs/heads/main/security/university-of-padua-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Research Data
- Library
- Repository
- Italy
---
