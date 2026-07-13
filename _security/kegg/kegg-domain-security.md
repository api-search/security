---
api_specs:
- filename: kegg-rest-api.yml
  format: yaml
  label: KEGG REST API
  slug: kegg-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kegg/refs/heads/main/openapi/kegg-rest-api.yml
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
