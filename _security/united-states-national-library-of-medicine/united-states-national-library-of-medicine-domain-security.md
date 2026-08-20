---
api_specs:
- filename: united-states-national-library-of-medicine-blast-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine BLAST API
  slug: united-states-national-library-of-medicine-blast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-blast-api-openapi.yml
- filename: united-states-national-library-of-medicine-fetch-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Fetch API
  slug: united-states-national-library-of-medicine-fetch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-fetch-api-openapi.yml
- filename: united-states-national-library-of-medicine-gene-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Gene API
  slug: united-states-national-library-of-medicine-gene-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-gene-api-openapi.yml
- filename: united-states-national-library-of-medicine-genome-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Genome API
  slug: united-states-national-library-of-medicine-genome-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-genome-api-openapi.yml
- filename: united-states-national-library-of-medicine-info-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Info API
  slug: united-states-national-library-of-medicine-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-info-api-openapi.yml
- filename: united-states-national-library-of-medicine-link-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Link API
  slug: united-states-national-library-of-medicine-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-link-api-openapi.yml
- filename: united-states-national-library-of-medicine-metadata-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Metadata API
  slug: united-states-national-library-of-medicine-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-metadata-api-openapi.yml
- filename: united-states-national-library-of-medicine-search-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Search API
  slug: united-states-national-library-of-medicine-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-search-api-openapi.yml
- filename: united-states-national-library-of-medicine-studies-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Studies API
  slug: united-states-national-library-of-medicine-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-studies-api-openapi.yml
- filename: united-states-national-library-of-medicine-taxonomy-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Taxonomy API
  slug: united-states-national-library-of-medicine-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-taxonomy-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  - 0 issue "entrust.net"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nih.gov
  spf: false
hosts:
- cert_expires: Sep 26 14:06:42 2026 GMT
  host: www.ncbi.nlm.nih.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 14:06:42 2026 GMT
  host: eutils.ncbi.nlm.nih.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 14:06:42 2026 GMT
  host: api.ncbi.nlm.nih.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: United States National Library Of Medicine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United States National Library of Medicine, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: United States National Library of Medicine
provider_slug: united-states-national-library-of-medicine
slug: united-states-national-library-of-medicine-domain-security
source_filename: united-states-national-library-of-medicine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eutils.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: null\ndomains:\n- domain: nih.gov\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"godaddy.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/security/united-states-national-library-of-medicine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal-Government
- Biomedical Research
- Healthcare
- Genomics
- Literature
---
