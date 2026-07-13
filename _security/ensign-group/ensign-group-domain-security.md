---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ensigngroup.net
  spf: true
hosts:
- cert_expires: Sep 12 07:09:28 2026 GMT
  host: www.ensigngroup.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.ensigngroup.net
  https: false
- host: api.ensigngroup.net
  https: false
kind: domain-security
layout: security
method: probed
name: Ensign Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ensign Group, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ensign Group
provider_slug: ensign-group
slug: ensign-group-domain-security
source_filename: ensign-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ensigngroup.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 07:09:28 2026 GMT\n  hsts: false\n- host: developer.ensigngroup.net\n  https: false\n- host: api.ensigngroup.net\n  https: false\ndomains:\n- domain: ensigngroup.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ensign-group/refs/heads/main/security/ensign-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Senior Living
- Healthcare
- Post-Acute
---
