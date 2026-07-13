---
api_specs:
- filename: ku-leuven-rdr.yaml
  format: yaml
  label: KU Leuven Research Data Repository (RDR) API
  slug: rdr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ku-leuven/refs/heads/main/openapi/ku-leuven-rdr.yaml
description: ''
domains:
- caa:
  - 0 iodef "mailto:abuse@kuleuven.be"
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kuleuven.be
  spf: true
hosts:
- cert_expires: Oct 23 20:53:06 2026 GMT
  host: www.kuleuven.be
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 20:37:44 2026 GMT
  host: rdr.kuleuven.be
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 23 20:42:41 2026 GMT
  host: admin.kuleuven.be
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ku Leuven Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KU Leuven, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KU Leuven
provider_slug: ku-leuven
slug: ku-leuven-domain-security
source_filename: ku-leuven-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kuleuven.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 20:53:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rdr.kuleuven.be\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 20:37:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: admin.kuleuven.be\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 20:42:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kuleuven.be\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:abuse@kuleuven.be\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ku-leuven/refs/heads/main/security/ku-leuven-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- Belgium
- Europe
---
