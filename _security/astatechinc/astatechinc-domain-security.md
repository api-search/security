---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: astatechinc.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.astatechinc.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Astatechinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astatechinc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Astatechinc
provider_slug: astatechinc
slug: astatechinc-domain-security
source_filename: astatechinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.astatechinc.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: astatechinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astatechinc/refs/heads/main/security/astatechinc-domain-security.yml
summary_line: TLSv1.2
tags:
- Contract Research Organization
- Pharmaceutical
- Custom Synthesis
- Bulk Manufacturing
- Analytical Services
- Catalog Products
---
