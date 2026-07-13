---
api_specs:
- filename: nvd-cve-openapi.yml
  format: yaml
  label: NVD CVE API
  slug: nvd-cve
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/openapi/nvd-cve-openapi.yml
- filename: nvd-cve-openapi.yml
  format: yaml
  label: NVD CVE Change History API
  slug: nvd-cve-history
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/openapi/nvd-cve-openapi.yml
- filename: nvd-cve-openapi.yml
  format: yaml
  label: NVD CPE API
  slug: nvd-cpe
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/openapi/nvd-cve-openapi.yml
- filename: nvd-cve-openapi.yml
  format: yaml
  label: NVD CPE Match Criteria API
  slug: nvd-cpe-match
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/openapi/nvd-cve-openapi.yml
- filename: nvd-cve-openapi.yml
  format: yaml
  label: NVD Source API
  slug: nvd-source
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/openapi/nvd-cve-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nist.gov
  spf: true
hosts:
- cert_expires: Sep 30 12:26:14 2026 GMT
  host: nvd.nist.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 14:16:22 2026 GMT
  host: services.nvd.nist.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nvd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NVD, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NVD
provider_slug: nvd
slug: nvd-domain-security
source_filename: nvd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nvd.nist.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:26:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.nvd.nist.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 14:16:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nist.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nvd/refs/heads/main/security/nvd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- CVE
- CPE
- Vulnerability
- CVSS
---
