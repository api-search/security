---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brandywinerealty.com
  spf: true
hosts:
- cert_expires: Sep 11 01:04:24 2026 GMT
  host: www.brandywinerealty.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brandywine Realty Trust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brandywine Realty Trust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brandywine Realty Trust
provider_slug: brandywine-realty-trust
slug: brandywine-realty-trust-domain-security
source_filename: brandywine-realty-trust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brandywinerealty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 01:04:24 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: brandywinerealty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandywine-realty-trust/refs/heads/main/security/brandywine-realty-trust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commercial Real Estate
- Life Science Real Estate
- Mixed Use Development
- Office
- Philadelphia
- REIT
- Real Estate
---
