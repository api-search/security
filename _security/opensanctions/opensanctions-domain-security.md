---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@opensanctions.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opensanctions.org
  spf: true
hosts:
- cert_expires: Aug 17 04:53:20 2026 GMT
  host: www.opensanctions.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opensanctions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenSanctions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenSanctions
provider_slug: opensanctions
slug: opensanctions-domain-security
source_filename: opensanctions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opensanctions.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 04:53:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opensanctions.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@opensanctions.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensanctions/refs/heads/main/security/opensanctions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- Public APIs
---
