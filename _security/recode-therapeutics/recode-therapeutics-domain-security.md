---
api_specs:
- filename: recode-therapeutics-content-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics Content API
  slug: recode-therapeutics-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-content-api-openapi.yml
- filename: recode-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics Discovery API
  slug: recode-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-discovery-api-openapi.yml
- filename: recode-therapeutics-embed-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics Embed API
  slug: recode-therapeutics-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-embed-api-openapi.yml
- filename: recode-therapeutics-media-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics Media API
  slug: recode-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-media-api-openapi.yml
- filename: recode-therapeutics-people-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics People API
  slug: recode-therapeutics-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-people-api-openapi.yml
- filename: recode-therapeutics-search-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics Search API
  slug: recode-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-search-api-openapi.yml
- filename: recode-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics Taxonomy API
  slug: recode-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: recodetx.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  - 0 iodef "mailto:caa@wordpress.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Sep 13 17:41:43 2026 GMT
  host: recodetx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Recode Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReCode Therapeutics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ReCode Therapeutics
provider_slug: recode-therapeutics
slug: recode-therapeutics-domain-security
source_filename: recode-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  Only recodetx.com is a ReCode Therapeutics host. developer.wordpress.org / wordpress.org appear\n  because the API entry's humanURL points at the upstream WordPress REST Handbook — the contract\n  this content API implements — and the prober walks every host in apis.yml. Read the\n  wordpress.org rows as upstream context, not as ReCode Therapeutics' posture.\nfindings:\n  - recodetx.com serves TLS 1.3 with a valid certificate but sends NO Strict-Transport-Security header.\n  - No DNSSEC on recodetx.com.\n  - No CAA records on recodetx.com — any CA may issue for the domain.\n  - SPF and DMARC are both published, but the DMARC policy is p=none — monitoring only, no enforcement against spoofed mail.\nhosts:\n- host: recodetx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 17:41:43 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https:\
  \ true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: recodetx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/security/recode-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- genetic-medicines
- biotechnology
- biopharmaceuticals
- mrna
- gene-correction
- lipid-nanoparticles
- drug-delivery
- rare-disease
- cystic-fibrosis
- primary-ciliary-dyskinesia
- clinical-trials
- life-sciences
- content-api
---
