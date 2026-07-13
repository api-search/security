---
api_specs:
- filename: national-library-of-medicine-openapi.yml
  format: yaml
  label: National Library of Medicine E-utilities
  slug: national-library-of-medicine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-library-of-medicine/refs/heads/main/openapi/national-library-of-medicine-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  - 0 issue "entrust.net"
  - 0 issue "godaddy.com"
  dmarc: false
  dnssec: true
  domain: nih.gov
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: www.nlm.nih.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
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
kind: domain-security
layout: security
method: probed
name: National Library Of Medicine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Library of Medicine, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: National Library of Medicine
provider_slug: national-library-of-medicine
slug: national-library-of-medicine-domain-security
source_filename: national-library-of-medicine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eutils.ncbi.nlm.nih.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:06:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nih.gov\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-library-of-medicine/refs/heads/main/security/national-library-of-medicine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Federal Government
- Health
- Library
- Medicine
---
