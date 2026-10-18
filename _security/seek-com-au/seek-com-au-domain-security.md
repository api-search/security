---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: seek.com.au
  spf: true
hosts:
- cert_expires: Nov 17 05:37:54 2026 GMT
  host: www.seek.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Seek Com Au Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SEEK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SEEK
provider_slug: seek-com-au
slug: seek-com-au-domain-security
source_filename: seek-com-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seek.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 05:37:54 2026 GMT\n  hsts: null\ndomains:\n- domain: seek.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seek-com-au/refs/heads/main/security/seek-com-au-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
