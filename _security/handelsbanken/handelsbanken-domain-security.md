---
description: ''
domains:
- caa:
  - 0 iodef "mailto:sirt@handelsbanken.se"
  - 0 issuewild ";"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: handelsbanken.se
  spf: true
hosts:
- cert_expires: Apr  3 23:59:59 2027 GMT
  host: handelsbanken.se
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Handelsbanken Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Handelsbanken, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Handelsbanken
provider_slug: handelsbanken
slug: handelsbanken-domain-security
source_filename: handelsbanken-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: handelsbanken.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: handelsbanken.se\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:sirt@handelsbanken.se\"\n  - 0 issuewild \";\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handelsbanken/refs/heads/main/security/handelsbanken-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Banking
- Finance
- Sweden
- Open Banking
---
