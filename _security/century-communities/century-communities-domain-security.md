---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: centurycommunities.com
  spf: true
hosts:
- cert_expires: Aug 24 05:44:50 2026 GMT
  host: www.centurycommunities.com
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
- host: developer.centurycommunities.com
  https: false
- host: api.centurycommunities.com
  https: false
kind: domain-security
layout: security
method: probed
name: Century Communities Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Century Communities, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Century Communities
provider_slug: century-communities
slug: century-communities-domain-security
source_filename: century-communities-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.centurycommunities.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 05:44:50 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\n- host: developer.centurycommunities.com\n  https: false\n- host: api.centurycommunities.com\n  https: false\ndomains:\n- domain: centurycommunities.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/century-communities/refs/heads/main/security/century-communities-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Homebuilding
---
