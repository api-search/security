---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rubicon.com
  spf: true
hosts:
- cert_expires: Sep 18 08:38:08 2026 GMT
  host: www.rubicon.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rubicon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rubicon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Rubicon
provider_slug: rubicon
slug: rubicon-domain-security
source_filename: rubicon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rubicon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:38:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: rubicon.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rubicon/refs/heads/main/security/rubicon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Waste Management
- Recycling
- Sustainability
- Circular Economy
- Fleet Management
- Smart City
- Enterprise
- Gated API
---
