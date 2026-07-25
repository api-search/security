---
api_specs:
- filename: kegg-conv-api-openapi.yml
  format: yaml
  label: Kyoto Encyclopedia of Genes and Genomes (KEGG) conv API
  slug: kegg-conv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kegg/refs/heads/main/openapi/kegg-conv-api-openapi.yml
- filename: kegg-ddi-api-openapi.yml
  format: yaml
  label: Kyoto Encyclopedia of Genes and Genomes (KEGG) ddi API
  slug: kegg-ddi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kegg/refs/heads/main/openapi/kegg-ddi-api-openapi.yml
- filename: kegg-find-api-openapi.yml
  format: yaml
  label: Kyoto Encyclopedia of Genes and Genomes (KEGG) find API
  slug: kegg-find-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kegg/refs/heads/main/openapi/kegg-find-api-openapi.yml
- filename: kegg-get-api-openapi.yml
  format: yaml
  label: Kyoto Encyclopedia of Genes and Genomes (KEGG) get API
  slug: kegg-get-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kegg/refs/heads/main/openapi/kegg-get-api-openapi.yml
- filename: kegg-info-api-openapi.yml
  format: yaml
  label: Kyoto Encyclopedia of Genes and Genomes (KEGG) info API
  slug: kegg-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kegg/refs/heads/main/openapi/kegg-info-api-openapi.yml
- filename: kegg-link-api-openapi.yml
  format: yaml
  label: Kyoto Encyclopedia of Genes and Genomes (KEGG) link API
  slug: kegg-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kegg/refs/heads/main/openapi/kegg-link-api-openapi.yml
- filename: kegg-list-api-openapi.yml
  format: yaml
  label: Kyoto Encyclopedia of Genes and Genomes (KEGG) list API
  slug: kegg-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kegg/refs/heads/main/openapi/kegg-list-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kegg.jp
  spf: true
hosts:
- cert_expires: Sep 12 19:04:39 2026 GMT
  host: www.kegg.jp
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 29 19:39:16 2026 GMT
  host: rest.kegg.jp
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kegg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kyoto Encyclopedia of Genes and Genomes (KEGG), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kyoto Encyclopedia of Genes and Genomes (KEGG)
provider_slug: kegg
slug: kegg-domain-security
source_filename: kegg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kegg.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 12 19:04:39 2026 GMT\n  hsts: false\n- host: rest.kegg.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 29 19:39:16 2026 GMT\n  hsts: false\ndomains:\n- domain: kegg.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kegg/refs/heads/main/security/kegg-domain-security.yml
summary_line: TLSv1.2
tags:
- Bioinformatics
- Genomics
- Life Sciences
- Pathways
- Metabolomics
- Drug Targets
- Disease
- Chemical Compounds
- Enzymes
- Orthology
---
