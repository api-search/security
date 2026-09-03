---
api_specs:
- filename: university-of-bonn-datasets-api-openapi.yml
  format: yaml
  label: University of Bonn Datasets API
  slug: university-of-bonn-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-bonn/refs/heads/main/openapi/university-of-bonn-datasets-api-openapi.yml
- filename: university-of-bonn-info-api-openapi.yml
  format: yaml
  label: University of Bonn Info API
  slug: university-of-bonn-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-bonn/refs/heads/main/openapi/university-of-bonn-info-api-openapi.yml
- filename: university-of-bonn-metrics-api-openapi.yml
  format: yaml
  label: University of Bonn Metrics API
  slug: university-of-bonn-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-bonn/refs/heads/main/openapi/university-of-bonn-metrics-api-openapi.yml
- filename: university-of-bonn-search-api-openapi.yml
  format: yaml
  label: University of Bonn Search API
  slug: university-of-bonn-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-bonn/refs/heads/main/openapi/university-of-bonn-search-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:sicherheitsteam@uni-bonn.de"
  - 0 issue "pki.dfn.de"
  - 0 issuewild "pki.dfn.de"
  - 0 issue "sectigo.com"
  - 0 issue "harica.gr"
  - 0 issuewild "harica.gr"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uni-bonn.de
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dataverse.org
  spf: true
hosts:
- cert_expires: Nov  7 22:00:31 2026 GMT
  host: www.uni-bonn.de
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: guides.dataverse.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 12:33:30 2027 GMT
  host: bonndata.uni-bonn.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Bonn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Bonn, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Bonn
provider_slug: university-of-bonn
slug: university-of-bonn-domain-security
source_filename: university-of-bonn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uni-bonn.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 22:00:31 2026 GMT\n  hsts: null\n- host: guides.dataverse.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: false\n- host: bonndata.uni-bonn.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 12:33:30 2027 GMT\n  hsts: false\ndomains:\n- domain: uni-bonn.de\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:sicherheitsteam@uni-bonn.de\"\n  - 0 issue \"pki.dfn.de\"\n  - 0 issuewild \"pki.dfn.de\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"harica.gr\"\n  - 0 issuewild \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: dataverse.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-bonn/refs/heads/main/security/university-of-bonn-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- University
- Higher Education
- Education
- Germany
- Public Research University
- Research Data
- Open Data
- Open Science
- Institutional Repository
- Dataverse
- OAI-PMH
- Identity Federation
- Shibboleth
- DFN-AAI
- Research Computing
- Scholarly Publishing
---
