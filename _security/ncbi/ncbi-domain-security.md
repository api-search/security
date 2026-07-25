---
api_specs:
- filename: ncbi-biosample-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) BioSample API
  slug: ncbi-biosample-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-biosample-api-openapi.yml
- filename: ncbi-gene-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Gene API
  slug: ncbi-gene-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-gene-api-openapi.yml
- filename: ncbi-genome-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Genome API
  slug: ncbi-genome-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-genome-api-openapi.yml
- filename: ncbi-organelle-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Organelle API
  slug: ncbi-organelle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-organelle-api-openapi.yml
- filename: ncbi-prokaryote-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Prokaryote API
  slug: ncbi-prokaryote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-prokaryote-api-openapi.yml
- filename: ncbi-taxonomy-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Taxonomy API
  slug: ncbi-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-taxonomy-api-openapi.yml
- filename: ncbi-version-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Version API
  slug: ncbi-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-version-api-openapi.yml
- filename: ncbi-virus-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Virus API
  slug: ncbi-virus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-virus-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "identrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  dmarc: false
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
  host: blast.ncbi.nlm.nih.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ncbi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Center for Biotechnology Information (NCBI), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: National Center for Biotechnology Information (NCBI)
provider_slug: ncbi
slug: ncbi-domain-security
source_filename: ncbi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eutils.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: blast.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nih.gov\n  dnssec: true\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"identrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/security/ncbi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Bioinformatics
- Genomics
- Life Sciences
- PubMed
- Sequences
- BLAST
- Taxonomy
- Chemistry
- Open Access
---
