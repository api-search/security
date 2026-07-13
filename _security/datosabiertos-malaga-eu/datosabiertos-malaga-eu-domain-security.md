---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: malaga.eu
  spf: true
hosts:
- cert_expires: Feb  9 11:17:05 2027 GMT
  host: datosabiertos.malaga.eu
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Datosabiertos Malaga Eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portal Datos Abiertos Ayuntamiento de Málaga, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Portal Datos Abiertos Ayuntamiento de Málaga
provider_slug: datosabiertos-malaga-eu
slug: datosabiertos-malaga-eu-domain-security
source_filename: datosabiertos-malaga-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datosabiertos.malaga.eu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  9 11:17:05 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: malaga.eu\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datosabiertos-malaga-eu/refs/heads/main/security/datosabiertos-malaga-eu-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Spain
---
