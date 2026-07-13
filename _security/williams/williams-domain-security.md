---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: williams.com
  spf: true
hosts:
- cert_expires: Sep 28 03:18:56 2026 GMT
  host: www.williams.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 17:54:43 2026 GMT
  host: www.1line.williams.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Williams Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Williams Companies, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Williams Companies
provider_slug: williams
slug: williams-domain-security
source_filename: williams-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.williams.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 03:18:56 2026 GMT\n  hsts: false\n- host: www.1line.williams.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 17:54:43 2026 GMT\n  hsts: false\ndomains:\n- domain: williams.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/williams/refs/heads/main/security/williams-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Natural Gas
- Pipeline
- Infrastructure
- Fortune 500
- Midstream
- Utilities
---
