---
api_specs:
- filename: vulncheck-api-openapi.json
  format: json
  label: VulnCheck API
  slug: vulncheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vulncheck/refs/heads/main/openapi/vulncheck-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vulncheck.com
  spf: true
hosts:
- cert_expires: Nov 25 13:00:01 2026 GMT
  host: www.vulncheck.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 13:51:45 2026 GMT
  host: docs.vulncheck.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.vulncheck.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Vulncheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VulnCheck, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VulnCheck
provider_slug: vulncheck
slug: vulncheck-domain-security
source_filename: vulncheck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vulncheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 13:00:01 2026 GMT\n  hsts: false\n- host: docs.vulncheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 13:51:45 2026 GMT\n  hsts: false\n- host: api.vulncheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: vulncheck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vulncheck/refs/heads/main/security/vulncheck-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Vulnerability Intelligence
- Exploit Intelligence
- Threat Intelligence
- Cybersecurity
- CVE
- Vulnerability Management
- Data
---
