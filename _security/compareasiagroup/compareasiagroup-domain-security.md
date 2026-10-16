---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 iodef "mailto:tech-admin@moneyherogroup.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: moneyherogroup.com
  spf: true
hosts:
- cert_expires: Apr 20 23:59:59 2027 GMT
  host: www.moneyherogroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Compareasiagroup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Compareasiagroup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Compareasiagroup
provider_slug: compareasiagroup
slug: compareasiagroup-domain-security
source_filename: compareasiagroup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moneyherogroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: moneyherogroup.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 iodef \"mailto:tech-admin@moneyherogroup.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/compareasiagroup/refs/heads/main/security/compareasiagroup-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Comparison
- Asia
- FinTech
---
