---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: groupon.com
  spf: true
hosts:
- cert_expires: Aug 23 10:41:14 2026 GMT
  host: www.groupon.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Groupon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for groupon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: groupon
provider_slug: groupon
slug: groupon-domain-security
source_filename: groupon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.groupon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 10:41:14 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: groupon.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groupon/refs/heads/main/security/groupon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fortune 1000
---
