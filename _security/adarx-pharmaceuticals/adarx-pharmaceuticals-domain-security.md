---
api_specs:
- filename: adarx-pharmaceuticals-clinics-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Clinics API
  slug: adarx-pharmaceuticals-clinics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-clinics-api-openapi.yml
- filename: adarx-pharmaceuticals-content-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Content API
  slug: adarx-pharmaceuticals-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-content-api-openapi.yml
- filename: adarx-pharmaceuticals-embed-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Embed API
  slug: adarx-pharmaceuticals-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-embed-api-openapi.yml
- filename: adarx-pharmaceuticals-index-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Index API
  slug: adarx-pharmaceuticals-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-index-api-openapi.yml
- filename: adarx-pharmaceuticals-media-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Media API
  slug: adarx-pharmaceuticals-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-media-api-openapi.yml
- filename: adarx-pharmaceuticals-people-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals People API
  slug: adarx-pharmaceuticals-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-people-api-openapi.yml
- filename: adarx-pharmaceuticals-search-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Search API
  slug: adarx-pharmaceuticals-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-search-api-openapi.yml
- filename: adarx-pharmaceuticals-taxonomy-api-openapi.yml
  format: yaml
  label: ADARx Pharmaceuticals Taxonomy API
  slug: adarx-pharmaceuticals-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/openapi/adarx-pharmaceuticals-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  caa_detail: No CAA record. Any public CA may issue for this domain.
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=100; rua=mailto:dmarc-reports@adarx.com; fo=1
  dnssec: true
  dnssec_detail: Two DS records present, algorithm 13 (ECDSAP256SHA256).
  domain: adarx.com
  spf: true
  spf_record: v=spf1 ip4:12.236.144.50 ip4:176.53.157.130 include:spf.protection.outlook.com include:sent-via.netsuite.com -all
- caa: []
  caa_detail: No CAA record.
  dmarc: true
  dmarc_detail: Delegated via CNAME to Proofpoint Email Defense.
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; fo=1; rua=mailto:dmarc_rua@emaildefense.proofpoint.com; ruf=mailto:dmarc_ruf@emaildefense.proofpoint.com;
  dnssec: true
  dnssec_detail: One DS record present, algorithm 13 (ECDSAP256SHA256).
  domain: stophae.com
  spf: true
  spf_detail: A hard-fail null SPF — the domain declares it sends no mail at all. Good hygiene for a site-only domain.
  spf_record: v=spf1 -all
hosts:
- cert_expires: Jan 15 22:56:16 2027 GMT
  host: www.adarx.com
  hsts: false
  https: true
  security_headers:
    note: nosniff is present on REST responses. No Strict-Transport-Security, no Content-Security-Policy and no X-Frame-Options were returned on the document root.
    x_content_type_options: nosniff
  server: Apache
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:30:44 2026 GMT
  host: stophae.com
  hsts: false
  https: true
  note: Fronted by Cloudflare. www.stophae.com does not resolve — the apex is the only valid host.
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adarx Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADARx Pharmaceuticals, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ADARx Pharmaceuticals
provider_slug: adarx-pharmaceuticals
slug: adarx-pharmaceuticals-domain-security
source_filename: adarx-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: >-\n  Live DNS (dig) and TLS/HTTP HEAD probes of the hosts ADARx Pharmaceuticals actually controls, run\n  on 2026-08-06. The upstream documentation host developer.wordpress.org, which appears as a\n  humanURL on the content API because it defines the wp/v2 contract, is deliberately excluded — it\n  is not an ADARx property and its posture says nothing about this provider.\nhosts:\n- host: www.adarx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 22:56:16 2027 GMT\n  hsts: false\n  server: Apache\n  security_headers:\n    x_content_type_options: nosniff\n    note: >-\n      nosniff is present on REST responses. No Strict-Transport-Security, no Content-Security-Policy\n      and no X-Frame-Options were returned on the document root.\n- host: stophae.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:30:44 2026 GMT\n  hsts: false\n  server: cloudflare\n  note: >-\n    Fronted by Cloudflare.\
  \ www.stophae.com does not resolve — the apex is the only valid host.\ndomains:\n- domain: adarx.com\n  dnssec: true\n  dnssec_detail: Two DS records present, algorithm 13 (ECDSAP256SHA256).\n  caa: []\n  caa_detail: No CAA record. Any public CA may issue for this domain.\n  spf: true\n  spf_record: 'v=spf1 ip4:12.236.144.50 ip4:176.53.157.130 include:spf.protection.outlook.com include:sent-via.netsuite.com -all'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1; p=quarantine; pct=100; rua=mailto:dmarc-reports@adarx.com; fo=1'\n- domain: stophae.com\n  dnssec: true\n  dnssec_detail: One DS record present, algorithm 13 (ECDSAP256SHA256).\n  caa: []\n  caa_detail: No CAA record.\n  spf: true\n  spf_record: 'v=spf1 -all'\n  spf_detail: >-\n    A hard-fail null SPF — the domain declares it sends no mail at all. Good hygiene for a\n    site-only domain.\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: 'v=DMARC1; p=reject; fo=1; rua=mailto:dmarc_rua@emaildefense.proofpoint.com;\
  \ ruf=mailto:dmarc_ruf@emaildefense.proofpoint.com;'\n  dmarc_detail: Delegated via CNAME to Proofpoint Email Defense.\nsummary:\n  strong:\n  - DNSSEC signed on both domains.\n  - SPF and DMARC published on both; stophae.com is at p=reject with a null SPF.\n  - TLS 1.3 on both hosts, certificates valid.\n  gaps:\n  - No CAA record on either domain — any public CA may issue.\n  - No HSTS on either host.\n  - adarx.com DMARC is p=quarantine rather than p=reject.\n  - No security.txt on either host (see well-known/adarx-pharmaceuticals-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adarx-pharmaceuticals/refs/heads/main/security/adarx-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- biopharmaceuticals
- RNA Therapeutics
- siRNA
- RNA Editing
- Clinical Trials
- Rare Disease
- Drug Development
- Life Sciences
- San Diego
- content-api
---
