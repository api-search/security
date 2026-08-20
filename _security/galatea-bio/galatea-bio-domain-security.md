---
api_specs:
- filename: galatea-bio-octopod-openapi.yml
  format: yaml
  label: Octopod Ancestry API
  slug: octopod-ancestry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/openapi/galatea-bio-octopod-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: galatea.bio
  spf: true
hosts:
- cert_expires: Nov 10 10:11:25 2026 GMT
  host: galatea.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 06:55:40 2026 GMT
  host: docs.galatea.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 11:00:23 2026 GMT
  host: api.galatea.bio
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Galatea Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Galatea Bio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Galatea Bio
provider_slug: galatea-bio
slug: galatea-bio-domain-security
source_filename: galatea-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: galatea.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 10:11:25 2026 GMT\n  hsts: false\n- host: docs.galatea.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:55:40 2026 GMT\n  hsts: false\n- host: api.galatea.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 11:00:23 2026 GMT\n  hsts: null\ndomains:\n- domain: galatea.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galatea-bio/refs/heads/main/security/galatea-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Genomics
- Bioinformatics
- Ancestry
- Precision Medicine
- polygenic-risk-score
- Clinical Laboratory
- Genetic Testing
- Biobank
- Life Sciences
- Health
- Sequencing
---
