---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dreamfindershomes.com
  spf: true
hosts:
- cert_expires: Sep 26 07:24:20 2026 GMT
  host: www.dreamfindershomes.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dream Finders Homes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dream Finders Homes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dream Finders Homes
provider_slug: dream-finders-homes
slug: dream-finders-homes-domain-security
source_filename: dream-finders-homes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dreamfindershomes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 07:24:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: dreamfindershomes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dream-finders-homes/refs/heads/main/security/dream-finders-homes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Homebuilding
- Real Estate
- Construction
- Residential
- Housing
---
