---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: imls.gov
  spf: true
hosts:
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: www.imls.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Institute Of Museum And Library Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Institute of Museum and Library Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Institute of Museum and Library Services
provider_slug: institute-of-museum-and-library-services
slug: institute-of-museum-and-library-services-domain-security
source_filename: institute-of-museum-and-library-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.imls.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: imls.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/institute-of-museum-and-library-services/refs/heads/main/security/institute-of-museum-and-library-services-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Grants
- Libraries
- Museums
---
