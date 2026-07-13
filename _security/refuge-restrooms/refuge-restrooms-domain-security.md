---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: refugerestrooms.org
  spf: false
hosts:
- cert_expires: Aug 19 23:10:26 2026 GMT
  host: www.refugerestrooms.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Refuge Restrooms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REFUGE Restrooms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: REFUGE Restrooms
provider_slug: refuge-restrooms
slug: refuge-restrooms-domain-security
source_filename: refuge-restrooms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.refugerestrooms.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:10:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: refugerestrooms.org\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refuge-restrooms/refs/heads/main/security/refuge-restrooms-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Transportation
- Public APIs
---
