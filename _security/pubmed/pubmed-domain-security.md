---
api_specs:
- filename: pubmed-history-api-openapi.yml
  format: yaml
  label: PubMed History API
  slug: pubmed-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-history-api-openapi.yml
- filename: pubmed-info-api-openapi.yml
  format: yaml
  label: PubMed Info API
  slug: pubmed-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-info-api-openapi.yml
- filename: pubmed-links-api-openapi.yml
  format: yaml
  label: PubMed Links API
  slug: pubmed-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-links-api-openapi.yml
- filename: pubmed-retrieval-api-openapi.yml
  format: yaml
  label: PubMed Retrieval API
  slug: pubmed-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-retrieval-api-openapi.yml
- filename: pubmed-search-api-openapi.yml
  format: yaml
  label: PubMed Search API
  slug: pubmed-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-search-api-openapi.yml
- filename: pubmed-summary-api-openapi.yml
  format: yaml
  label: PubMed Summary API
  slug: pubmed-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-summary-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "identrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nih.gov
  spf: true
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
  host: pmc.ncbi.nlm.nih.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pubmed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PubMed, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: PubMed
provider_slug: pubmed
slug: pubmed-domain-security
source_filename: pubmed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eutils.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pmc.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nih.gov\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"identrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/security/pubmed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- biomedical
- life science
- research
- literature
- citations
- abstracts
- MeSH
- genomics
- PubMed
- NCBI
---
