---
api_specs:
- filename: ucsc-genomic-data-genomes-api-openapi.yml
  format: yaml
  label: UCSC Genomic Data Genomes API
  slug: ucsc-genomic-data-genomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsc-genomic-data/refs/heads/main/openapi/ucsc-genomic-data-genomes-api-openapi.yml
- filename: ucsc-genomic-data-hubs-api-openapi.yml
  format: yaml
  label: UCSC Genomic Data Hubs API
  slug: ucsc-genomic-data-hubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsc-genomic-data/refs/heads/main/openapi/ucsc-genomic-data-hubs-api-openapi.yml
- filename: ucsc-genomic-data-search-api-openapi.yml
  format: yaml
  label: UCSC Genomic Data Search API
  slug: ucsc-genomic-data-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsc-genomic-data/refs/heads/main/openapi/ucsc-genomic-data-search-api-openapi.yml
- filename: ucsc-genomic-data-sequences-api-openapi.yml
  format: yaml
  label: UCSC Genomic Data Sequences API
  slug: ucsc-genomic-data-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsc-genomic-data/refs/heads/main/openapi/ucsc-genomic-data-sequences-api-openapi.yml
- filename: ucsc-genomic-data-tracks-api-openapi.yml
  format: yaml
  label: UCSC Genomic Data Tracks API
  slug: ucsc-genomic-data-tracks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsc-genomic-data/refs/heads/main/openapi/ucsc-genomic-data-tracks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ucsc.edu
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: genome.ucsc.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.genome.ucsc.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: genome-euro.ucsc.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ucsc Genomic Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UCSC Genomic Data, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UCSC Genomic Data
provider_slug: ucsc-genomic-data
slug: ucsc-genomic-data-domain-security
source_filename: ucsc-genomic-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genome.ucsc.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\n- host: api.genome.ucsc.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\n- host: genome-euro.ucsc.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ucsc.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucsc-genomic-data/refs/heads/main/security/ucsc-genomic-data-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Genomics
- Bioinformatics
- DNA
- Biology
- Research
- Open Science
---
