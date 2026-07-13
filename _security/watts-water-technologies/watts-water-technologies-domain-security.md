---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wattswater.com
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.wattswater.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.wattswater.com
  https: false
- host: api.wattswater.com
  https: false
kind: domain-security
layout: security
method: probed
name: Watts Water Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Watts Water Technologies, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Watts Water Technologies
provider_slug: watts-water-technologies
slug: watts-water-technologies-domain-security
source_filename: watts-water-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wattswater.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\n- host: developer.wattswater.com\n  https: false\n- host: api.wattswater.com\n  https: false\ndomains:\n- domain: wattswater.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/watts-water-technologies/refs/heads/main/security/watts-water-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Water
- Industrial
- Infrastructure
---
