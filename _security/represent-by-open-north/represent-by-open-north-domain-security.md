---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opennorth.ca
  spf: true
hosts:
- cert_expires: Sep  6 12:32:29 2026 GMT
  host: represent.opennorth.ca
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Represent By Open North Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Represent by Open North, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Represent by Open North
provider_slug: represent-by-open-north
slug: represent-by-open-north-domain-security
source_filename: represent-by-open-north-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: represent.opennorth.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  6 12:32:29 2026 GMT\n  hsts: false\ndomains:\n- domain: opennorth.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/represent-by-open-north/refs/heads/main/security/represent-by-open-north-domain-security.yml
summary_line: TLSv1.2
tags:
- Government
- Public APIs
---
