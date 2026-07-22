---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: iaventures.com
  spf: true
hosts:
- cert_expires: Sep 27 06:41:52 2026 GMT
  host: www.iaventures.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ia Ventures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IA Ventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: IA Ventures
provider_slug: ia-ventures
slug: ia-ventures-domain-security
source_filename: ia-ventures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iaventures.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:41:52 2026 GMT\n  hsts: false\ndomains:\n- domain: iaventures.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ia-ventures/refs/heads/main/security/ia-ventures-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Venture Capital
- Early Stage
- Seed
- Fintech
- Data
- New York
---
