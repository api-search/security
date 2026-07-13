---
api_specs:
- filename: university-of-york-white-rose-research-oai.yaml
  format: yaml
  label: White Rose Research Online (OAI-PMH)
  slug: white-rose-research-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-york/refs/heads/main/openapi/university-of-york-white-rose-research-oai.yaml
- filename: university-of-york-white-rose-etheses-oai.yaml
  format: yaml
  label: White Rose eTheses Online (OAI-PMH)
  slug: white-rose-etheses-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-york/refs/heads/main/openapi/university-of-york-white-rose-etheses-oai.yaml
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuevmc ";"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issuemail "pki.goog"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: york.ac.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: whiterose.ac.uk
  spf: true
hosts:
- cert_expires: Sep  5 15:34:42 2026 GMT
  host: www.york.ac.uk
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: eprints.whiterose.ac.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: etheses.whiterose.ac.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of York Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of York, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of York
provider_slug: university-of-york
slug: university-of-york-domain-security
source_filename: university-of-york-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.york.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 15:34:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: eprints.whiterose.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: etheses.whiterose.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: york.ac.uk\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuevmc \";\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuemail \"pki.goog\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: whiterose.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-york/refs/heads/main/security/university-of-york-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- United Kingdom
- Research
- Library
- Open Access
- OAI-PMH
---
