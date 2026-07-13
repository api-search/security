---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: donneesquebec.ca
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.donneesquebec.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Donneesquebec Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Donnees Quebec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Donnees Quebec
provider_slug: donneesquebec-ca
slug: donneesquebec-ca-domain-security
source_filename: donneesquebec-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.donneesquebec.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: donneesquebec.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/donneesquebec-ca/refs/heads/main/security/donneesquebec-ca-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Provincial Government
- Canada
---
