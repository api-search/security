---
description: ''
domains:
- caa:
  - 0 issue "symantec.com"
  - 0 iodef "mailto:hostmaster@intermedia.net"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intermedia.com
  spf: true
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "geotrust.com"
  - 0 issue "amazon.com"
  - 0 iodef "mailto:ssl@intermedia.net"
  - 0 issue "symantec.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intermedia.net
  spf: true
hosts:
- cert_expires: Sep 16 04:01:37 2026 GMT
  host: www.intermedia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: developer.intermedia.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intermedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intermedia, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Intermedia
provider_slug: intermedia
slug: intermedia-domain-security
source_filename: intermedia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.intermedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:01:37 2026 GMT\n  hsts: false\n- host: developer.intermedia.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: intermedia.com\n  dnssec: false\n  caa:\n  - 0 issue \"symantec.com\"\n  - 0 iodef \"mailto:hostmaster@intermedia.net\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: intermedia.net\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:ssl@intermedia.net\"\n  - 0 issue \"symantec.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intermedia/refs/heads/main/security/intermedia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud
- Communications
- Contact Center
- Video Conferencing
- Voice
---
