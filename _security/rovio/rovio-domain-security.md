---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rovio.com
  spf: true
hosts:
- cert_expires: Jan  9 16:00:11 2027 GMT
  host: www.rovio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rovio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rovio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rovio
provider_slug: rovio
slug: rovio-domain-security
source_filename: rovio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rovio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 16:00:11 2027 GMT\n  hsts: false\ndomains:\n- domain: rovio.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rovio/refs/heads/main/security/rovio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Gaming
- Mobile Games
- Entertainment
- Games
---
