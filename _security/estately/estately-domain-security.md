---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "comodo.com"
  - 0 issue "comodoca.com"
  - 0 iodef "mailto:ops@estately.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: estately.com
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: estately.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Estately Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Estately, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Estately
provider_slug: estately
slug: estately-domain-security
source_filename: estately-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: estately.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: estately.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"comodo.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 iodef \"mailto:ops@estately.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/estately/refs/heads/main/security/estately-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Real Estate
- Homes for Sale
- MLS
- Property Search
- RETS
- Open Source
---
