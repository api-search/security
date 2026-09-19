---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ingredion.com
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: myingredion.com
  note: 'Portal-only domain: no SPF, DMARC, CAA or DS records published. Mail for the company is sent from ingredion.com, which does publish SPF and DMARC.'
  spf: false
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: www.ingredion.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  cert_subject_cn: myingredion.com
  cert_subject_o: Ingredion Incorporated
  host: myingredion.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: MyIngredion customer portal (Salesforce Experience Cloud). TLS certificate is issued to O=Ingredion Incorporated, L=Westchester, ST=Illinois — first-party ownership confirmed.
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Ingredion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ingredion, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ingredion
provider_slug: ingredion
slug: ingredion-domain-security
source_filename: ingredion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts; MyIngredion portal host added by the enrichment\n  pass\nhosts:\n- host: www.ingredion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: myingredion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  cert_subject_o: Ingredion Incorporated\n  cert_subject_cn: myingredion.com\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: MyIngredion customer portal (Salesforce Experience Cloud). TLS certificate is issued to O=Ingredion\n    Incorporated, L=Westchester, ST=Illinois — first-party ownership confirmed.\ndomains:\n- domain: ingredion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: myingredion.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy:\
  \ null\n  note: 'Portal-only domain: no SPF, DMARC, CAA or DS records published. Mail for the company is sent\n    from ingredion.com, which does publish SPF and DMARC.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ingredion/refs/heads/main/security/ingredion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Food and Beverage
- Ingredients
- Food Manufacturing
- Agriculture
- Plant-Based Proteins
- Specialty Chemicals
- Consumer Packaged Goods
---
