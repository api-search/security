---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: republic-services.com
  spf: true
hosts:
- cert_expires: Sep 13 18:46:38 2026 GMT
  host: www.republic-services.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Republic Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Republic Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Republic Services
provider_slug: republic-services
slug: republic-services-domain-security
source_filename: republic-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.republic-services.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:46:38 2026 GMT\n  hsts: false\ndomains:\n- domain: republic-services.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/republic-services/refs/heads/main/security/republic-services-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Environmental Services
- Fortune 500
- Recycling
- Waste Management
---
