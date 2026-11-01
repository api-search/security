---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: europa.eu
  spf: true
hosts:
- cert_expires: Mar 25 23:59:59 2027 GMT
  host: data.ecb.europa.eu
  hsts: true
  hsts_max_age: 86500
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: European Central Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ECB Data Portal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: ECB Data Portal
provider_slug: european-central-bank
slug: european-central-bank-domain-security
source_filename: european-central-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.ecb.europa.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86500\ndomains:\n- domain: europa.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/european-central-bank/security/european-central-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Finance
- Banking
- European Union
- Economic Data
- Statistics
- Open Data
---
