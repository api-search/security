---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: creatorcabins.com
  spf: true
hosts:
- cert_expires: Sep 13 08:50:09 2026 GMT
  host: creatorcabins.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Creator Cabins Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creator Cabins, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Creator Cabins
provider_slug: creator-cabins
slug: creator-cabins-domain-security
source_filename: creator-cabins-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: creatorcabins.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:50:09 2026 GMT\n  hsts: false\ndomains:\n- domain: creatorcabins.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creator-cabins/refs/heads/main/security/creator-cabins-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto Web3
- Coliving
- Community
- DAO
- Network City
- Real Estate
---
