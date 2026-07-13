---
description: ''
domains:
- caa:
  - 0 issue "d-trust.net"
  - 0 issue "godaddy.com"
  - 0 iodef "mailto:dataportpki@dataport.de"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: schleswig-holstein.de
  spf: true
hosts:
- cert_expires: Aug 29 13:51:51 2026 GMT
  host: opendata.schleswig-holstein.de
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendata Schleswig Holstein De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Data Schleswig-Holstein, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Open Data Schleswig-Holstein
provider_slug: opendata-schleswig-holstein-de
slug: opendata-schleswig-holstein-de-domain-security
source_filename: opendata-schleswig-holstein-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.schleswig-holstein.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 13:51:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: schleswig-holstein.de\n  dnssec: true\n  caa:\n  - 0 issue \"d-trust.net\"\n  - 0 issue \"godaddy.com\"\n  - 0 iodef \"mailto:dataportpki@dataport.de\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-schleswig-holstein-de/refs/heads/main/security/opendata-schleswig-holstein-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- State Government
- Germany
---
